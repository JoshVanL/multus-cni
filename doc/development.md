## Development Information

## How do I submit an issue?

Use GitHub as normally, you'll be presented with an option to submit a issue or enhancement request.

Issues are considered stale after 90 days. After which, the maintainers reserve the right to close an issue.

Typically, we'll tag the submitter and ask for more information if necessary before closing.

If an issue is closed that you don't feel is sufficiently resolved, please feel free to re-open the issue and provide any necessary information.

## How do I build multus-cni?

You can use the built in `./build` script!

```
git clone https://github.com/intel/multus-cni.git
cd multus-cni
./build
```

## How do I run CI tests?

Multus has go unit tests (based on ginkgo framework).The following commands drive CI tests manually in your environment:

```
sudo ./test.sh
```

## What are the best practices for logging?

The following are the best practices for multus logging:

* Add `logging.Debugf()` at the begining of functions
* In case of error handling, use `logging.Errorf()` with given error info
* `logging.Panicf()` only be used for critical errors (it should NOT normally be used)


## CI Introduction

TBD
