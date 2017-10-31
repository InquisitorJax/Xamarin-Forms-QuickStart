# Xamarin-Forms-QuickStart
.NET Standard Bare bones Xamarin Forms Android, iOS and UWP project template

## .NET Standard Library Support for Xamarin
https://blog.xamarin.com/net-standard-library-support-for-xamarin/

Targets .NET standard 2 - which adds support for Xamarin iOS, Android and Windows UWP

Note that if you still want to have PCL dependencies, then you need to update the project.json file to contain an 'imports' statement.
It should look something like: (already done in the source code)
```json
{
"supports": {},    
    "dependencies": {
    "Microsoft.NETCore.Portable.Compatibility": "1.0.1",
    "NETStandard.Library": "1.6.0"
  },
  "frameworks": {
    "netstandard2.0": {
      "imports": "portable-net45+wp80+win8+wpa81"
   }
  }
}
```

For information on .NET Standard libraries:
https://blogs.infosupport.com/sharing-code-across-net-platforms-with-net-standard/
