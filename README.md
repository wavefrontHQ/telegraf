
[Read the plugin doc](/plugins/outputs/wavefront/README.md)

## Creating Your Own Telegraf Builds With The Wavefront Plugin

#### 1. Get the plugin:
```
> go get github.com/wavefronthq/telegraf/plugins/outputs/wavefront
```


#### 2. Include the plugin:

Add this line to the `import` section of your `$TELEGRAF_HOME/plugins/outputs/all/all.go` file:
```
_ "github.com/wavefronthq/telegraf/plugins/outputs/wavefront"
```

You should now be able to use the default Telegraf `Makefile` to create builds/packages. The Wavefront output plugin will be included in the
Telegraf binary.