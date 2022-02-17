# Conclusions from work, Jan 04 - Feb 17

## Go Environment

1. GOPATH is where we store go environment
2. GOROOT is where we put projects
3. When compiling local project, using make static is enough, but need to specify GO111MODULE=off
4. gdb can be used to debug

## Packages and functions

1. """log.Printf()""" only accecpt string, fmt.Sprint() would be a good choice
2. """log.Printf()""" only accecpt string, if we have numbers, function laike """strconv.FormatInt()""" should be considered
3. most golang functions return two variables, value and error
4. to print the error, error.Error() which is a string
5. to get the domain from libvirt.Domain, GetName() and GetUUIDString() are very helpful
6. interface {} is the original type
7. golang has anonymous functions, using it properly
8. golang has pointers, which is helpful and powerful, but using it carefully!

## Telegraf

1. Config files defines the behaviors of Telegraf
2. To test a certain plugin, commenting out the useless plugins should be considered