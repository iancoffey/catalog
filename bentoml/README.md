# BentoML

This task allows operations on BentoML services.

## Parameters

* **YATAISERVICE**: Optional address of YataiService to connect to for command.

  _default_: ""`

* **ARGS**: The arguments to pass to `bentoml` CLI. This parameter is required to run this task.

### Examples

Run `bentoml --help` for BentoML usage. Using the [Tekton CLI](https://github.com/tektoncd/cli/blob/master/docs/cmd/tkn_task_start.md) (`tkn`):

Use bentoml to retrieve a full ML build environment in the cwd:

```shell
tkn task start bentoml -p ARGS="retrieve ServiceName:20200616152703_9E2AD7","YATAISERVICE=10.10.10.1:50051 --target_dir=/workspace/storage"
```
