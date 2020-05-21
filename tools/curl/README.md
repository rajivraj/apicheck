Apicheck from CURL
==================

This tool provide a binray curl command (acurl) that will be translated into a
valid reqres object. 

*Tool type:* generator

## Tool description

You can use this way:

The binary curl command accept the same parameters than the curl command. For 
further documentation you can check curl man:

```bash
$ man curl
```

This tool add curl_log field to the _meta data. You can find all curl internal
log info in this field.

## Quick start

### With APICheck Package Manager

As simple as use curl:

```bash
$ apc install acurl
$ eval $(apc activate)
(APICheck) $ acurl www.google.com
```

You can use to retrieve also ssl protected urls:

```bash
(APICheck) $ acurl https://www.google.com
```

### With Docker

```bash
$ docker run -it --rm bbvalabs/acurl www.google.com
```