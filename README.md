# shell history in erlang shell

Let each node maintain their own shell history storage. By the way, enable by default.

## use

Use erlc to compile group_history.erl, and then copy the beam file into erlang install path($ERLANG\_INSTALL\_PATH/lib/kernel-$VSN/ebin/).

```bash
git co 21.1
erlc group_history.erl
export erl_kernel_bin=~/.erlvm/ver/otp_21.1/lib/erlang/lib/kernel-6.1/ebin
mv $erl_kernel_bin/group_history.beam $erl_kernel_bin/group_history.beam-backup
cp group_history.erl $erl_kernel_bin/
```

## vsn

otp-21.1
otp-22.3
otp-23.0

