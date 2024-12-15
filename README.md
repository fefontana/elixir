# elixir
Elixir fundamentals on Erlang VM.
https://hexdocs.pm/elixir/introduction.html

Type:

i@loveyou:~/coding$iex

(linux command for interactive mode), or load you source code with:

i@loveyou:~/coding$elixir simple.exs

Interactive Elixir (1.12.2) - press Ctrl+C to exit (type h() ENTER for help)

iex(1)> 1+48
49

iex(3)> h()
                                  IEx.Helpers                                   

Welcome to Interactive Elixir. You are currently seeing the documentation for
the module IEx.Helpers which provides many helpers to make Elixir's shell more
joyful to work with.

This message was triggered by invoking the helper h(), usually referred to as
h/0 (since it expects 0 arguments).

You can use the h/1 function to invoke the documentation for any Elixir module
or function:

    iex> h(Enum)
    iex> h(Enum.map)
    iex> h(Enum.reverse/1)

You can also use the i/1 function to introspect any value you have in the
shell:

    iex> i("hello")

There are many other helpers available, here are some examples:

  • b/1            - prints callbacks info and docs for a given module
  • c/1            - compiles a file
  • c/2            - compiles a file and writes bytecode to the given path
  • cd/1           - changes the current directory
  • clear/0        - clears the screen
  • exports/1      - shows all exports (functions + macros) in a module
  • flush/0        - flushes all messages sent to the shell
  • h/0            - prints this help message
  • h/1            - prints help for the given module, function or macro
  • i/0            - prints information about the last value
  • i/1            - prints information about the given term
  • ls/0           - lists the contents of the current directory
  • ls/1           - lists the contents of the specified directory
  • open/1         - opens the source for the given module or function in
    your editor
  • pid/1          - creates a PID from a string
  • pid/3          - creates a PID with the 3 integer arguments passed
  • port/1         - creates a port from a string
  • port/2         - creates a port with the 2 non-negative integers passed
  • ref/1          - creates a reference from a string
  • ref/4          - creates a reference with the 4 integer arguments
    passed
  • pwd/0          - prints the current working directory
  • r/1            - recompiles the given module's source file
  • recompile/0    - recompiles the current project
  • runtime_info/0 - prints runtime info (versions, memory usage, stats)
  • v/0            - retrieves the last value from the history
  • v/1            - retrieves the nth value from the history

Help for all of those functions can be consulted directly from the command line
using the h/1 helper itself. Try:

    iex> h(v/0)

To list all IEx helpers available, which is effectively all exports (functions
and macros) in the IEx.Helpers module:

    iex> exports(IEx.Helpers)

This module also includes helpers for debugging purposes, see IEx.break!/4 for
more information.

To learn more about IEx as a whole, type h(IEx).


--------------------------------------------------------------------------------------

CTRL+C

i FOR INFO
l FOR VIEW LOADED _______

--------------------------------------------------------------------------------------

iex(4)> 
BREAK: (a)bort (A)bort with dump (c)ontinue (p)roc info (i)nfo
       (l)oaded (v)ersion (k)ill (D)b-tables (d)istribution
i
=memory
total: 22159248
processes: 4969840
processes_used: 4969840
system: 17189408
atom: 327857
atom_used: 318137
binary: 334928
code: 8393550
ets: 440056
=hash_table:atom_tab
size: 8192
used: 6277
objs: 12102
depth: 9
=index_table:atom_tab
size: 12288
limit: 1048576
entries: 12103
=hash_table:module_code
size: 128
used: 101
objs: 183
depth: 5
=index_table:module_code
size: 1024
limit: 65536
entries: 183
=hash_table:export_list
size: 4096
used: 2871
objs: 4976
depth: 7
=index_table:export_list
size: 5120
limit: 524288
entries: 4976
=hash_table:export_list
size: 4096
used: 2867
objs: 4967
depth: 7
=hash_table:process_reg
size: 32
used: 19
objs: 33
depth: 4
=hash_table:fun_table
size: 1024
used: 729
objs: 1180
depth: 6
=hash_table:node_table
size: 16
used: 1
objs: 1
depth: 1
=hash_table:dist_table
size: 16
used: 1
objs: 1
depth: 1
=allocated_areas
sys_misc: 57816
static: 2107328
atom_space: 163880 154160
atom_table: 163977
module_table: 100368
export_table: 221604
export_list: 995200
register_table: 372
fun_table: 8306
module_refs: 8736
loaded_code: 7059336
dist_table: 635
node_table: 291
bits_bufs_size: 0
bif_timer: 0
process_table: 3145728
port_table: 786432
ets_misc: 131072
external_alloc: 7059336
=allocator:sys_alloc
option e: true
option m: libc
option tt: 131072
option tp: 0
=allocator:temp_alloc[0]
versions: 2.1 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 90
option rsbcmt: 80
option rmbcmt: 100
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option mbsd: 3
option as: gf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 5 5
mbcs blocks[temp_alloc] size: 0 10904 10904
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
temp_alloc calls: 901
temp_free calls: 901
temp_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:temp_alloc[1]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 90
option rsbcmt: 80
option rmbcmt: 100
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: af
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 5 5
mbcs blocks[temp_alloc] size: 0 639032 639032
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 2 2
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 1179648 1179648
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
temp_alloc calls: 12468
temp_free calls: 12468
temp_realloc calls: 33
mseg_alloc calls: 4
mseg_dealloc calls: 4
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:temp_alloc[2]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 90
option rsbcmt: 80
option rmbcmt: 100
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: af
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 1 1
mbcs blocks[temp_alloc] size: 0 1904 1904
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
temp_alloc calls: 2
temp_free calls: 2
temp_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:temp_alloc[3]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 90
option rsbcmt: 80
option rmbcmt: 100
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: af
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 1 1
mbcs blocks[temp_alloc] size: 0 56 56
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
temp_alloc calls: 1
temp_free calls: 1
temp_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:temp_alloc[4]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 90
option rsbcmt: 80
option rmbcmt: 100
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: af
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 1 1
mbcs blocks[temp_alloc] size: 0 1904 1904
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
temp_alloc calls: 2
temp_free calls: 2
temp_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:temp_alloc[5]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 90
option rsbcmt: 80
option rmbcmt: 100
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: af
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 1 1
mbcs blocks[temp_alloc] size: 0 56 56
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
temp_alloc calls: 1
temp_free calls: 1
temp_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:temp_alloc[6]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 90
option rsbcmt: 80
option rmbcmt: 100
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: af
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 1 1
mbcs blocks[temp_alloc] size: 0 56 56
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
temp_alloc calls: 1
temp_free calls: 1
temp_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:temp_alloc[7]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 90
option rsbcmt: 80
option rmbcmt: 100
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: af
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 1 1
mbcs blocks[temp_alloc] size: 0 56 56
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
temp_alloc calls: 1
temp_free calls: 1
temp_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:temp_alloc[8]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 90
option rsbcmt: 80
option rmbcmt: 100
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: af
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 5 5
mbcs blocks[temp_alloc] size: 0 21520 21520
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
temp_alloc calls: 1636
temp_free calls: 1636
temp_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:sl_alloc[0]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 80
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 76 76
mbcs blocks[sl_alloc] size: 0 37096 37096
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 2 2
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 294912 294912
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
sl_alloc calls: 596
sl_free calls: 596
sl_realloc calls: 0
mseg_alloc calls: 2
mseg_dealloc calls: 2
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:sl_alloc[1]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 80
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: S
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 6137 6137
mbcs blocks[sl_alloc] size: 0 1093424 1093424
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 3 3
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 1343488 1343488
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
sl_alloc calls: 11973
sl_free calls: 11973
sl_realloc calls: 59
mseg_alloc calls: 21
mseg_dealloc calls: 21
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:sl_alloc[2]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 80
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: S
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
sl_alloc calls: 0
sl_free calls: 0
sl_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:sl_alloc[3]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 80
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: S
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
sl_alloc calls: 0
sl_free calls: 0
sl_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:sl_alloc[4]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 80
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: S
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
sl_alloc calls: 0
sl_free calls: 0
sl_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:sl_alloc[5]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 80
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: S
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
sl_alloc calls: 0
sl_free calls: 0
sl_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:sl_alloc[6]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 80
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: S
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
sl_alloc calls: 0
sl_free calls: 0
sl_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:sl_alloc[7]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 80
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: S
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
sl_alloc calls: 0
sl_free calls: 0
sl_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:sl_alloc[8]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 80
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: S
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 202 202
mbcs blocks[sl_alloc] size: 0 315608 315608
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 3 3
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 1343488 1343488
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
sl_alloc calls: 458
sl_free calls: 458
sl_realloc calls: 0
mseg_alloc calls: 2
mseg_dealloc calls: 2
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:std_alloc[0]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 51 55 55
mbcs blocks[std_alloc] size: 137448 145344 145344
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 2 2 2
mbcs mseg carriers: 1
mbcs sys_alloc carriers: 1
mbcs carriers size: 294912 294912 294912
mbcs mseg carriers size: 262144
mbcs sys_alloc carriers size: 32768
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
std_alloc calls: 75
std_free calls: 24
std_realloc calls: 1
mseg_alloc calls: 1
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:std_alloc[1]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: D
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 169 171 171
mbcs blocks[std_alloc] size: 71696 78968 78968
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 2 2 2
mbcs mseg carriers: 1
mbcs sys_alloc carriers: 1
mbcs carriers size: 294912 294912 294912
mbcs mseg carriers size: 262144
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
std_alloc calls: 783
std_free calls: 614
std_realloc calls: 1
mseg_alloc calls: 1
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:std_alloc[2]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: D
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 2 2 2
mbcs blocks[std_alloc] size: 128 128 128
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
std_alloc calls: 2
std_free calls: 0
std_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:std_alloc[3]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: D
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 1 1 1
mbcs blocks[std_alloc] size: 64 64 64
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
std_alloc calls: 1
std_free calls: 0
std_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:std_alloc[4]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: D
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 1 1 1
mbcs blocks[std_alloc] size: 64 64 64
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
std_alloc calls: 1
std_free calls: 0
std_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:std_alloc[5]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: D
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 1 1 1
mbcs blocks[std_alloc] size: 64 64 64
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
std_alloc calls: 1
std_free calls: 0
std_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:std_alloc[6]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: D
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 1 1 1
mbcs blocks[std_alloc] size: 64 64 64
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
std_alloc calls: 1
std_free calls: 0
std_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:std_alloc[7]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: D
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 1 1 1
mbcs blocks[std_alloc] size: 64 64 64
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
std_alloc calls: 1
std_free calls: 0
std_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:std_alloc[8]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: D
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 1 2 2
mbcs blocks[std_alloc] size: 64 7232 7232
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
std_alloc calls: 13
std_free calls: 12
std_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ll_alloc[0]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
option rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 524288
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 3837 3842 3842
mbcs blocks[ll_alloc] size: 8776304 8810808 8810808
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 5 5 5
mbcs mseg carriers: 4
mbcs sys_alloc carriers: 1
mbcs carriers size: 9961472 9961472 9961472
mbcs mseg carriers size: 9437184
mbcs sys_alloc carriers size: 524288
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ll_alloc calls: 3843
ll_free calls: 6
ll_realloc calls: 0
mseg_alloc calls: 4
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ll_alloc[1]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
option rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 524288
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 85
option acnl: 1000
option acfml: 0
option cp: L
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 13688 13688 13688
mbcs blocks[ll_alloc] size: 1901992 1901992 1901992
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 4 4 4
mbcs mseg carriers: 3
mbcs sys_alloc carriers: 1
mbcs carriers size: 3932160 3932160 3932160
mbcs mseg carriers size: 3407872
mbcs sys_alloc carriers size: 524288
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ll_alloc calls: 13690
ll_free calls: 2
ll_realloc calls: 0
mseg_alloc calls: 3
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ll_alloc[2]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
opt
ion rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 524288
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 85
option acnl: 1000
option acfml: 0
option cp: L
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 524288 524288 524288
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 524288
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ll_alloc calls: 0
ll_free calls: 0
ll_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ll_alloc[3]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
option rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 524288
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 85
option acnl: 1000
option acfml: 0
option cp: L
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 524288 524288 524288
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 524288
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ll_alloc calls: 0
ll_free calls: 0
ll_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ll_alloc[4]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
option rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 524288
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 85
option acnl: 1000
option acfml: 0
option cp: L
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 524288 524288 524288
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 524288
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ll_alloc calls: 0
ll_free calls: 0
ll_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ll_alloc[5]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
option rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 524288
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 85
option acnl: 1000
option acfml: 0
option cp: L
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 524288 524288 524288
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 524288
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ll_alloc calls: 0
ll_free calls: 0
ll_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ll_alloc[6]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
option rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 524288
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 85
option acnl: 1000
option acfml: 0
option cp: L
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 524288 524288 524288
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 524288
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ll_alloc calls: 0
ll_free calls: 0
ll_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ll_alloc[7]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
option rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 524288
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 85
option acnl: 1000
option acfml: 0
option cp: L
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 524288 524288 524288
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 524288
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ll_alloc calls: 0
ll_free calls: 0
ll_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ll_alloc[8]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
option rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 524288
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 85
option acnl: 1000
option acfml: 0
option cp: L
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 1696 1696 1696
mbcs blocks[ll_alloc] size: 198824 198824 198824
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 524288 524288 524288
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 524288
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ll_alloc calls: 1696
ll_free calls: 0
ll_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:eheap_alloc[0]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 50
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 21 44 44
mbcs blocks[eheap_alloc] size: 305568 311184 311184
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 2 2 2
mbcs mseg carriers: 1
mbcs sys_alloc carriers: 1
mbcs carriers size: 393216 393216 393216
mbcs mseg carriers size: 262144
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
eheap_alloc calls: 53
eheap_free calls: 32
eheap_realloc calls: 0
mseg_alloc calls: 1
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:eheap_alloc[1]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 50
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 45
option acnl: 1000
option acfml: 0
option cp: H
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 77 81 81
mbcs blocks[eheap_alloc] size: 869544 1205504 1205504
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 3 3 3
mbcs mseg carriers: 2
mbcs sys_alloc carriers: 1
mbcs carriers size: 2228224 2228224 2228224
mbcs mseg carriers size: 2097152
mbcs sys_alloc carriers size: 131072
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 1 1 1
sbcs blocks[eheap_alloc] size: 600912 600912 600912
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 1 1 1
sbcs mseg carriers: 1
sbcs sys_alloc carriers: 0
sbcs carriers size: 602112 602112 602112
sbcs mseg carriers size: 602112
sbcs sys_alloc carriers size: 0
eheap_alloc calls: 839
eheap_free calls: 761
eheap_realloc calls: 62
mseg_alloc calls: 4
mseg_dealloc calls: 1
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:eheap_alloc[2]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 50
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 45
option acnl: 1000
option acfml: 0
option cp: H
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 2 2 2
mbcs blocks[eheap_alloc] size: 136 136 136
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
eheap_alloc calls: 2
eheap_free calls: 0
eheap_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:eheap_alloc[3]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 50
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 45
option acnl: 1000
option acfml: 0
option cp: H
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 1 1 1
mbcs blocks[eheap_alloc] size: 72 72 72
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
eheap_alloc calls: 1
eheap_free calls: 0
eheap_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:eheap_alloc[4]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 50
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 45
option acnl: 1000
option acfml: 0
option cp: H
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 1 1 1
mbcs blocks[eheap_alloc] size: 64 64 64
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
eheap_alloc calls: 1
eheap_free calls: 0
eheap_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:eheap_alloc[5]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 50
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 45
option acnl: 1000
option acfml: 0
option cp: H
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
eheap_alloc calls: 0
eheap_free calls: 0
eheap_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:eheap_alloc[6]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 50
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 45
option acnl: 1000
option acfml: 0
option cp: H
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
eheap_alloc calls: 0
eheap_free calls: 0
eheap_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:eheap_alloc[7]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 50
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 45
option acnl: 1000
option acfml: 0
option cp: H
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 1 1 1
mbcs blocks[eheap_alloc] size: 72 72 72
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
eheap_alloc calls: 1
eheap_free calls: 0
eheap_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:eheap_alloc[8]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 50
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 45
option acnl: 1000
option acfml: 0
option cp: H
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 7 7
mbcs blocks[eheap_alloc] size: 0 49152 49152
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
eheap_alloc calls: 8
eheap_free calls: 8
eheap_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ets_alloc[0]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 0 0 0
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 0
mbcs carriers size: 0 0 0
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ets_alloc calls: 0
ets_free calls: 0
ets_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 0
sys_free calls: 0
sys_realloc calls: 0
=allocator:ets_alloc[1]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: E
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 607 607 607
mbcs blocks[ets_alloc] size: 308984 308984 308984
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 3 3 3
mbcs mseg carriers: 2
mbcs sys_alloc carriers: 1
mbcs carriers size: 1343488 1343488 1343488
mbcs mseg carriers size: 1310720
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ets_alloc calls: 611
ets_free calls: 4
ets_realloc calls: 8
mseg_alloc calls: 2
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ets_alloc[2]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: E
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ets_alloc calls: 0
ets_free calls: 0
ets_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ets_alloc[3]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: E
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ets_alloc calls: 0
ets_free calls: 0
ets_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ets_alloc[4]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: E
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ets_alloc calls: 0
ets_free calls: 0
ets_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ets_alloc[5]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: E
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ets_alloc calls: 0
ets_free calls: 0
ets_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ets_alloc[6]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: E
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ets_alloc calls: 0
ets_free calls: 0
ets_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ets_alloc[7]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: E
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ets_alloc calls: 0
ets_free calls: 0
ets_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ets_alloc[8]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: E
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ets_alloc calls: 0
ets_free calls: 0
ets_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:fix_alloc[0]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
fix type: enif_select_data_state 0 0
fix type: driver_select_data_state 0 0
fix type: link 0 0
fix type: monitor 0 0
fix type: sl_thr_q_element 0 0
fix type: magic_indirection 0 0
fix type: nsched_pid_ref_entry 0 0
fix type: nsched_magic_ref_entry 0 0
fix type: bif_timer 0 0
fix type: hl_ptimer 0 0
fix type: ll_ptimer 0 0
fix type: msg_ref 0 0
fix type: receive_marker_block 0 0
fix type: proc 4464 4464
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 6 33 33
mbcs blocks[fix_alloc] size: 4512 6240 6240
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
fix_alloc calls: 174
fix_free calls: 168
fix_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:fix_alloc[1]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: F
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 179 218 218
mbcs blocks[fix_alloc] size: 46880 53776 53776
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 2 2 2
mbcs mseg carriers: 1
mbcs sys_alloc carriers: 1
mbcs carriers size: 294912 294912 294912
mbcs mseg carriers size: 262144
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
fix_alloc calls: 481
fix_free calls: 302
fix_realloc calls: 0
mseg_alloc calls: 1
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:fix_alloc[2]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: F
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
fix_alloc calls: 0
fix_free calls: 0
fix_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:fix_alloc[3]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: F
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
fix_alloc calls: 0
fix_free calls: 0
fix_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:fix_alloc[4]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: F
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
fix_alloc calls: 0
fix_free calls: 0
fix_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:fix_alloc[5]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: F
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
fix_alloc calls: 0
fix_free calls: 0
fix_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:fix_alloc[6]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: F
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
fix_alloc calls: 0
fix_free calls: 0
fix_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:fix_alloc[7]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: F
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
fix_alloc calls: 0
fix_free calls: 0
fix_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:fix_alloc[8]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: F
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
fix_alloc calls: 0
fix_free calls: 0
fix_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:literal_alloc
versions: 0.9 3.0
option e: true
option t: false
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
option rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 1048576
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aobf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 203 203 203
mbcs blocks[literal_alloc] size: 1496240 1496240 1496240
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 2 2 2
mbcs mseg carriers: 2
mbcs sys_alloc carriers: 0
mbcs carriers size: 2097152 2097152 2097152
mbcs mseg carriers size: 2097152
mbcs sys_alloc carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
literal_alloc calls: 209
literal_free calls: 6
literal_realloc calls: 0
mseg_alloc calls: 2
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 0
sys_free calls: 0
sys_realloc calls: 0
=allocator:binary_alloc[0]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 8 54 54
mbcs blocks[binary_alloc] size: 316008 1558776 1558776
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 3 4 4
mbcs mseg carriers: 2
mbcs sys_alloc carriers: 1
mbcs carriers size: 1343488 3440640 3440640
mbcs mseg carriers size: 1310720
mbcs sys_alloc carriers size: 32768
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 1 1
sbcs blocks[binary_alloc] size: 0 917448 917448
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 1 1
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 917504 917504
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
binary_alloc calls: 368
binary_free calls: 360
binary_realloc calls: 11
mseg_alloc calls: 21
mseg_dealloc calls: 19
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:binary_alloc[1]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: B
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 102 120 120
mbcs blocks[binary_alloc] size: 18920 37632 37632
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 2 2
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 294912 294912
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
binary_alloc calls: 940
binary_free calls: 838
binary_realloc calls: 67
mseg_alloc calls: 4
mseg_dealloc calls: 4
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:binary_alloc[2]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: B
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
binary_alloc calls: 0
binary_free calls: 0
binary_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:binary_alloc[3]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: B
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
binary_alloc calls: 0
binary_free calls: 0
binary_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:binary_alloc[4]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: B
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
binary_alloc calls: 0
binary_free calls: 0
binary_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:binary_alloc[5]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: B
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
binary_alloc calls: 0
binary_free calls: 0
binary_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:binary_alloc[6]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: B
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
binary_alloc calls: 0
binary_free calls: 0
binary_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:binary_alloc[7]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: B
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
binary_alloc calls: 0
binary_free calls: 0
binary_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:binary_alloc[8]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: B
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 14 14
mbcs blocks[binary_alloc] size: 0 7392 7392
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
binary_alloc calls: 14
binary_free calls: 14
binary_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:driver_alloc[0]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 39 39 39
mbcs blocks[driver_alloc] size: 7792 7792 7792
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
driver_alloc calls: 40
driver_free calls: 1
driver_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:driver_alloc[1]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: R
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 18 18 18
mbcs blocks[driver_alloc] size: 37432 37432 37432
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 2 2 2
mbcs mseg carriers: 1
mbcs sys_alloc carriers: 1
mbcs carriers size: 294912 294912 294912
mbcs mseg carriers size: 262144
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
driver_alloc calls: 31
driver_free calls: 13
driver_realloc calls: 0
mseg_alloc calls: 2
mseg_dealloc calls: 1
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:driver_alloc[2]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: R
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
driver_alloc calls: 0
driver_free calls: 0
driver_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:driver_alloc[3]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: R
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
driver_alloc calls: 0
driver_free calls: 0
driver_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:driver_alloc[4]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: R
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
driver_alloc calls: 0
driver_free calls: 0
driver_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:driver_alloc[5]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: R
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
driver_alloc calls: 0
driver_free calls: 0
driver_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:driver_alloc[6]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: R
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
driver_alloc calls: 0
driver_free calls: 0
driver_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:driver_alloc[7]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: R
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
driver_alloc calls: 0
driver_free calls: 0
driver_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:driver_alloc[8]
versions: 0.9 3.0
option e: true
option t: 9
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acnl: 1000
option acfml: 0
option cp: R
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
driver_alloc calls: 0
driver_free calls: 0
driver_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:test_alloc
option e: false
=allocator:mseg_alloc[0]
version: 0.9
option amcbf: 4194304
option rmcbf: 20
option mcs: 10
memory kind: all memory
cached_segments: 0
cache_hits: 17
segments: 8 9 9
segments_watermark: 8
segments_size: 11272192 13369344 13369344
mseg_alloc calls: 29
mseg_dealloc calls: 21
mseg_realloc calls: 0
mseg_create calls: 12
mseg_create_resize calls: 0
mseg_destroy calls: 4
mseg_recreate calls: 0
mseg_clear_cache calls: 0
mseg_check_cache calls: 5
=allocator:mseg_alloc[1]
version: 0.9
option amcbf: 4194304
option rmcbf: 20
option mcs: 10
memory kind: all memory
cached_segments: 0
cache_hits: 25
segments: 11 12 12
segments_watermark: 11
segments_size: 8204288 8466432 8466432
mseg_alloc calls: 42
mseg_dealloc calls: 31
mseg_realloc calls: 0
mseg_create calls: 17
mseg_create_resize calls: 0
mseg_destroy calls: 7
mseg_recreate calls: 0
mseg_clear_cache calls: 0
mseg_check_cache calls: 6
=allocator:mseg_alloc[2]
version: 0.9
option amcbf: 4194304
option rmcbf: 20
option mcs: 10
memory kind: all memory
cached_segments: 0
cache_hits: 0
segments: 0 0 0
segments_watermark: 0
segments_size: 0 0 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
mseg_create calls: 0
mseg_create_resize calls: 0
mseg_destroy calls: 0
mseg_recreate calls: 0
mseg_clear_cache calls: 0
mseg_check_cache calls: 0
=allocator:mseg_alloc[3]
version: 0.9
option amcbf: 4194304
option rmcbf: 20
option mcs: 10
memory kind: all memory
cached_segments: 0
cache_hits: 0
segments: 0 0 0
segments_watermark: 0
segments_size: 0 0 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
mseg_create calls: 0
mseg_create_resize calls: 0
mseg_destroy calls: 0
mseg_recreate calls: 0
mseg_clear_cache calls: 0
mseg_check_cache calls: 0
=allocator:mseg_alloc[4]
version: 0.9
option amcbf: 4194304
option rmcbf: 20
option mcs: 10
memory kind: all memory
cached_segments: 0
cache_hits: 0
segments: 0 0 0
segments_watermark: 0
segments_size: 0 0 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
mseg_create calls: 0
mseg_create_resize calls: 0
mseg_destroy calls: 0
mseg_recreate calls: 0
mseg_clear_cache calls: 0
mseg_check_cache calls: 0
=allocator:mseg_alloc[5]
version: 0.9
option amcbf: 4194304
option rmcbf: 20
option mcs: 10
memory kind: all memory
cached_segments: 0
cache_hits: 0
segments: 0 0 0
segments_watermark: 0
segments_size: 0 0 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
mseg_create calls: 0
mseg_create_resize calls: 0
mseg_destroy calls: 0
mseg_recreate calls: 0
mseg_clear_cache calls: 0
mseg_check_cache calls: 0
=allocator:mseg_alloc[6]
version: 0.9
option amcbf: 4194304
option rmcbf: 20
option mcs: 10
memory kind: all memory
cached_segments: 0
cache_hits: 0
segments: 0 0 0
segments_watermark: 0
segments_size: 0 0 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
mseg_create calls: 0
mseg_create_resize calls: 0
mseg_destroy calls: 0
mseg_recreate calls: 0
mseg_clear_cache calls: 0
mseg_check_cache calls: 0
=allocator:mseg_alloc[7]
version: 0.9
option amcbf: 4194304
option rmcbf: 20
option mcs: 10
memory kind: all memory
cached_segments: 0
cache_hits: 0
segments: 0 0 0
segments_watermark: 0
segments_size: 0 0 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
mseg_create calls: 0
mseg_create_resize calls: 0
mseg_destroy calls: 0
mseg_recreate calls: 0
mseg_clear_cache calls: 0
mseg_check_cache calls: 0
=allocator:mseg_alloc[8]
version: 0.9
option amcbf: 4194304
option rmcbf: 20
option mcs: 10
memory kind: all memory
cached_segments: 0
cache_hits: 0
segments: 0 2 2
segments_watermark: 0
segments_size: 0 1310720 1310720
mseg_alloc calls: 2
mseg_dealloc calls: 2
mseg_realloc calls: 0
mseg_create calls: 2
mseg_create_resize calls: 0
mseg_destroy calls: 2
mseg_recreate calls: 0
mseg_clear_cache calls: 0
mseg_check_cache calls: 2
=allocator:erts_mmap.default_mmap
option scs: 0
os mmap size used: 19476480
=allocator:erts_mmap.literal_mmap
option scs: 1073676288
option sco: true
option scrpm: false
option scrfsd: 1024
supercarrier total size: 1073741824
supercarrier total sa size: 2097152
supercarrier total sua size: 0
supercarrier used size: 2162688
supercarrier used sa size: 2097152
supercarrier used sua size: 0
supercarrier used free segs: 0
supercarrier max free segs: 0
supercarrier allocated free segs: 0
supercarrier reserved free segs: 1024
supercarrier sa free segs: 0
supercarrier sua free segs: 0
=allocator:alloc_util
option mmc: 18446744073709551615
option ycs: 1048576
option sac: true
=allocator:instr
option t: false

nil
iex(5)> 
BREAK: (a)bort (A)bort with dump (c)ontinue (p)roc info (i)nfo
       (l)oaded (v)ersion (k)ill (D)b-tables (d)istribution
l
Current code: 8525928
Old code: 0
erts_code_purger 16416
erl_init 2552
init 73616
prim_buffer 5480
prim_eval 1352
prim_inet 116024
prim_file 48248
zlib 27488
socket_registry 25136
prim_socket 58328
prim_net 7408
prim_zip 30616
erl_prim_loader 68216
erlang 121208
erts_internal 25896
erl_tracer 1720
erts_literal_area_collector 5544
erts_dirty_process_signal_handler 2520
atomics 3936
counters 4968
persistent_term 1576
ets 71128
erl_lint 349664
proc_lib 48832
lists 109696
erl_parse 310688
logger_simple_h 14456
supervisor 91768
filename 53048
gen_server 68384
gen 24088
gen_event 54512
erl_eval 111048
code_server 71784
application_controller 132632
code 47896
error_handler 5360
logger_filters 5200
file_io_server 56448
error_logger 18568
file 50120
logger 57016
kernel 17784
logger_server 36224
file_server 15056
logger_backend 7488
heart 18088
application_master 21440
logger_config 11272
application 11856
logger_proxy 9360
logger_olp 24760
queue 33696
proplists 16632
binary 41272
gb_sets 25544
gb_trees 17584
os 17928
unicode 51976
inet_db 82456
inet_config 26816
inet_udp 6248
inet 87584
inet_parse 46896
inet_gethost_native 35992
rpc 48024
global 103104
net_kernel 100248
erl_distribution 7392
global_group 54288
standard_error 10800
supervisor_bridge 20872
user_sup 5288
'Elixir.IEx.CLI' 8456
user_drv 40840
group 43584
edlin 34592
io_lib 44040
group_history 41776
io_lib_format 56304
timer 16632
kernel_config 7504
kernel_refc 6584
logger_sup 1616
logger_handler_watcher 3440
maps 20432
erl_signal_handler 3624
logger_formatter 30240
'Elixir.IEx' 9224
logger_std_h 29936
logger_h_common 26528
c 66424
orddict 10984
raw_file_io 4048
'Elixir.Application' 26664
epp 103784
erl_scan 91576
erl_anno 12456
eval_bits 33168
elixir 25848
string 140864
unicode_util 1016688
'Elixir.Kernel' 168352
'Elixir.Macro.Env' 6648
io 28800
'Elixir.System' 32672
'Elixir.String.Tokenizer' 112504
elixir_config 5576
elixir_sup 1712
elixir_code_server 10880
'Elixir.IEx.App' 1824
'Elixir.Supervisor' 19880
'Elixir.Keyword' 34648
'Elixir.Enum' 215816
'Elixir.Access' 25024
'Elixir.IEx.Config' 11208
'Elixir.IEx.Broker' 14088
'Elixir.IEx.Pry' 32944
'Elixir.Supervisor.Default' 1480
'Elixir.Agent' 12024
'Elixir.GenServer' 45864
'Elixir.Agent.Server' 5856
'Elixir.Process' 10688
'Elixir.IEx.Server' 21984
'Elixir.Logger' 22560
'Elixir.Logger.App' 6880
'Elixir.Logger.Watcher' 6976
'Elixir.Logger.BackendSupervisor' 5728
'Elixir.Logger.Config' 8408
'Elixir.Logger.Backends.Console' 17288
'Elixir.Logger.Formatter' 11448
'Elixir.Regex' 27800
re 45208
'Elixir.IO.ANSI' 47000
'Elixir.Logger.Handler' 14992
'Elixir.Map' 17888
'Elixir.Logger.Filter' 2592
'Elixir.Kernel.CLI' 48616
'Elixir.IO' 15816
'Elixir.List' 26032
'Elixir.IEx.Evaluator' 27008
'Elixir.IEx.History' 7752
elixir_env 17784
elixir_dispatch 26880
elixir_quote 36400
elixir_expand 162848
elixir_aliases 29184
'Elixir.IEx.Helpers' 50512
elixir_import 21928
ordsets 6072
elixir_erl_pass 50592
elixir_erl 47752
'Elixir.Path' 22960
'Elixir.File' 46256
elixir_utils 12184
'Elixir.Node' 5168
'Elixir.String.Chars' 6616
'Elixir.String.Chars.Integer' 1896
'Elixir.String' 66768
'Elixir.String.Chars.Atom' 1952
elixir_tokenizer 154112
elixir_parser 539488
elixir_locals 19288
elixir_rewrite 41440
erl_internal 15216
elixir_erl_var 6768
'Elixir.Inspect.Opts' 2224
'Elixir.Inspect.Algebra' 38824
'Elixir.Inspect' 6552
'Elixir.Inspect.Integer' 3664
io_lib_pretty 72384
elixir_errors 14464
'Elixir.SyntaxError' 4664
'Elixir.Exception' 47048
'Elixir.Code' 38152
'Elixir.Inspect.Atom' 2120
'Elixir.Code.Identifier' 20416
'Elixir.CompileError' 4664
'Elixir.IEx.Introspection' 64216
beam_lib 74696
'Elixir.IO.ANSI.Docs' 62472
'Elixir.String.Unicode' 114056
'Elixir.String.Break' 12376


D - TABLES


iex(6)> 
BREAK: (a)bort (A)bort with dump (c)ontinue (p)roc info (i)nfo
       (l)oaded (v)ersion (k)ill (D)b-tables (d)istribution
D 
=ets:<0.42.0>
Slot: 109377668874680
Table: logger
Name: logger
Buckets: 256
Chain Length Avg: 0.011719
Chain Length Max: 1
Chain Length Min: 0
Chain Length Std Dev: 0.107617
Chain Length Expected Std Dev: 0.108042
Fixed: false
84: [{'$primary_config$',#{filter_default=>log,filters=>[{process_disabled,{fun 'Elixir.Logger.Filter':process_disabled/2,[]}}],handlers=>['Elixir.Logger'],level=>debug,metadata=>#{}}}]
116: [{'$proxy_config$',#{burst_limit_enable=>false,burst_limit_max_count=>500,burst_limit_window_time=>1000,drop_mode_qlen=>1000,flush_qlen=>5000,overload_kill_enable=>false,overload_kill_mem_size=>3000000,overload_kill_qlen=>20000,overload_kill_restart_after=>5000,sync_mode_qlen=>500}}]
152: [{{'$handler_config$','Elixir.Logger'},#{config=>#{counter=>{atomics,#Ref<0.3590211226.1908801537.245335>},sasl=>false,thresholds=>{20,500},translators=>[{'Elixir.Logger.Translator',translate}],truncate=>8096,utc_log=>false},filter_default=>log,filters=>[],formatter=>{logger_formatter,#{}},id=>'Elixir.Logger',level=>all,module=>'Elixir.Logger.Handler'}}]
Objects: 3
Words: 1462
Type: set
Protection: protected
Compressed: false
Write Concurrency: true
Read Concurrency: true
=ets:<0.44.0>
Slot: 109377668886408
Table: ac_tab
Name: ac_tab
Buckets: 256
Chain Length Avg: 0.148438
Chain Length Max: 2
Chain Length Min: 0
Chain Length Std Dev: 0.376867
Chain Length Expected Std Dev: 0.384523
Fixed: false
1: [{{env,logger,backends},[console]}]
14: [{{loaded,compiler},{appl,compiler,{appl_data,compiler,[],undefined,[],[beam_a,beam_asm,beam_block,beam_call_types,beam_clean,beam_dict,beam_digraph,beam_disasm,beam_flatten,beam_jump,beam_kernel_to_ssa,beam_listing,beam_opcodes,beam_peep,beam_ssa,beam_ssa_bc_size,beam_ssa_bool,beam_ssa_bsm,beam_ssa_codegen,beam_ssa_dead,beam_ssa_funs,beam_ssa_lint,beam_ssa_opt,beam_ssa_pp,beam_ssa_pre_codegen,beam_ssa_recv,beam_ssa_share,beam_ssa_throw,beam_ssa_type,beam_trim,beam_types,beam_utils,beam_validator,beam_z,cerl,cerl_clauses,cerl_inline,cerl_trees,compile,core_scan,core_lint,core_parse,core_pp,core_lib,erl_bifs,rec_env,sys_core_alias,sys_core_bsm,sys_core_fold,sys_core_fold_lists,sys_core_inline,sys_core_prepare,sys_messages,sys_pre_attributes,v3_core,v3_kernel,v3_kernel_pp],infinity,infinity},"ERTS  CXC 138 10",[],"8.0.4",undefined,[],[],[kernel,stdlib]}}]
18: [{{env,elixir,check_endianness},true}]
22: [{{env,kernel,logger_sasl_compatible},false}]
40: [{{env,iex,default_prompt},<<"%prefix(%counter)>">>}]
53: [{{env,logger,utc_log},false}]
58: [{{env,kernel,logger_level},notice}]
63: [{{loaded,stdlib},{appl,stdlib,{appl_data,stdlib,[timer_server,rsh_starter,take_over_monitor,pool_master,dets],undefined,[],[array,base64,beam_lib,binary,c,calendar,dets,dets_server,dets_sup,dets_utils,dets_v9,dict,digraph,digraph_utils,edlin,edlin_expand,epp,eval_bits,erl_abstract_code,erl_anno,erl_bits,erl_compile,erl_error,erl_eval,erl_expand_records,erl_internal,erl_lint,erl_parse,erl_posix_msg,erl_pp,erl_scan,erl_stdlib_errors,erl_tar,error_logger_file_h,error_logger_tty_h,escript,ets,file_sorter,filelib,filename,gb_trees,gb_sets,gen,gen_event,gen_fsm,gen_server,gen_statem,io,io_lib,io_lib_format,io_lib_format_ryu_table,io_lib_fread,io_lib_pretty,lists,log_mf_h,maps,math,ms_transform,orddict,ordsets,otp_internal,pool,proc_lib,proplists,qlc,qlc_pt,queue,rand,random,re,sets,shell,shell_default,shell_docs,slave,sofs,string,supervisor,supervisor_bridge,sys,timer,unicode,unicode_util,uri_string,win32reg,zip],infinity,infinity},"ERTS  CXC 138 10",[],"3.17",undefined,[],[],[kernel]}}]
76: [{{env,logger,discard_threshold_periodic_check},30000}]
77: [{{env,kernel,shell_docs_ansi},auto}]
81: [{{application_master,iex},<0.88.0>},{{env,logger,compile_time_application},nil}]
91: [{{env,logger,compile_time_purge_matching},[]}]
102: [{{env,logger,sync_threshold},20}]
105: [{{env,logger,translator_inspect_opts},[]}]
116: [{{env,logger,console},[]}]
118: [{{env,iex,inspect},[{pretty,true}]},{{env,logger,discard_threshold},500}]
121: [{{env,logger,start_options},[]}]
123: [{{env,kernel,logger},[{handler,default,logger_std_h,#{config=>#{type=>standard_io},formatter=>{logger_formatter,#{legacy_header=>true,single_line=>false}}}}]}]
131: [{{env,logger,discard_threshold_for_error_logger},500}]
138: [{{loaded,iex},{appl,iex,{appl_data,iex,['Elixir.IEx.Broker','Elixir.IEx.Config','Elixir.IEx.Pry','Elixir.IEx.Supervisor'],undefined,{'Elixir.IEx.App',[]},['Elixir.IEx','Elixir.IEx.App','Elixir.IEx.Autocomplete','Elixir.IEx.Broker','Elixir.IEx.CLI','Elixir.IEx.Config','Elixir.IEx.Evaluator','Elixir.IEx.Helpers','Elixir.IEx.History','Elixir.IEx.Info','Elixir.IEx.Info.Any','Elixir.IEx.Info.Atom','Elixir.IEx.Info.BitString','Elixir.IEx.Info.Date','Elixir.IEx.Info.Float','Elixir.IEx.Info.Function','Elixir.IEx.Info.Integer','Elixir.IEx.Info.List','Elixir.IEx.Info.Map','Elixir.IEx.Info.NaiveDateTime','Elixir.IEx.Info.PID','Elixir.IEx.Info.Port','Elixir.IEx.Info.Reference','Elixir.IEx.Info.Time','Elixir.IEx.Info.Tuple','Elixir.IEx.Introspection','Elixir.IEx.Pry','Elixir.IEx.Server','Elixir.IEx.State'],infinity,infinity},"iex",[],"1.12.2",undefined,[],[],[kernel,stdlib,elixir]}}]
139: [{{application_master,kernel},<0.46.0>}]
145: [{{application_master,elixir},<0.82.0>}]
154: [{{env,iex,alive_prompt},<<"%prefix(%node)%counter>">>}]
159: [{{loaded,kernel},{appl,kernel,{appl_data,kernel,[application_controller,erl_reply,auth,boot_server,code_server,disk_log_server,disk_log_sup,erl_prim_loader,error_logger,file_server_2,fixtable_server,global_group,global_name_server,heart,init,kernel_config,kernel_refc,kernel_sup,logger,logger_handler_watcher,logger_sup,net_kernel,net_sup,rex,user,os_server,ddll_server,erl_epmd,inet_db,pg],undefined,{kernel,[]},[application,application_controller,application_master,application_starter,auth,code,code_server,dist_util,erl_boot_server,erl_compile_server,erl_distribution,erl_erts_errors,erl_reply,erl_kernel_errors,erl_signal_handler,erpc,error_handler,error_logger,file,file_server,file_io_server,global,global_group,global_search,group,group_history,heart,inet6_tcp,inet6_tcp_dist,inet6_udp,inet6_sctp,inet_config,inet_hosts,inet_gethost_native,inet_tcp_dist,kernel,kernel_config,kernel_refc,local_tcp,local_udp,logger,logger_backend,logger_config,logger_disk_log_h,logger_filters,logger_formatter,logger_h_common,logger_handler_watcher,logger_olp,logger_proxy,logger_server,logger_simple_h,logger_std_h,logger_sup,net,net_adm,net_kernel,os,ram_file,rpc,user,user_drv,user_sup,disk_log,disk_log_1,disk_log_server,disk_log_sup,dist_ac,erl_ddll,erl_epmd,erts_debug,gen_tcp,gen_tcp_socket,gen_udp,gen_udp_socket,gen_sctp,inet,inet_db,inet_dns,inet_parse,inet_res,inet_tcp,inet_udp,inet_sctp,pg,pg2,raw_file_io,raw_file_io_compressed,raw_file_io_deflate,raw_file_io_delayed,raw_file_io_inflate,raw_file_io_list,seq_trace,socket,standard_error,wrap_log_reader],infinity,infinity},"ERTS  CXC 138 10",[],"8.2",undefined,[],[],[]}}]
163: [{{env,logger,truncate},8096}]
170: [{{env,logger,handle_sasl_reports},false}]
172: [{{env,elixir,ansi_enabled},true}]
185: [{{loaded,logger},{appl,logger,{appl_data,logger,['Elixir.Logger','Elixir.Logger.BackendSupervisor','Elixir.Logger.Supervisor','Elixir.Logger.Watcher'],undefined,{'Elixir.Logger.App',[]},['Elixir.Logger','Elixir.Logger.App','Elixir.Logger.BackendSupervisor','Elixir.Logger.Backends.Console','Elixir.Logger.Config','Elixir.Logger.Filter','Elixir.Logger.Formatter','Elixir.Logger.Handler','Elixir.Logger.Translator','Elixir.Logger.Utils','Elixir.Logger.Watcher'],infinity,infinity},"logger",[],"1.12.2",undefined,[],[],[kernel,stdlib,elixir]}}]
196: [{{env,iex,history_size},20}]
197: [{{loaded,elixir},{appl,elixir,{appl_data,elixir,[elixir_sup,elixir_config,elixir_code_server],undefined,{elixir,[]},['Elixir.Access','Elixir.Agent.Server','Elixir.Agent','Elixir.Application','Elixir.ArgumentError','Elixir.ArithmeticError','Elixir.Atom','Elixir.BadArityError','Elixir.BadBooleanError','Elixir.BadFunctionError','Elixir.BadMapError','Elixir.BadStructError','Elixir.Base','Elixir.Behaviour','Elixir.Bitwise','Elixir.Calendar.ISO','Elixir.Calendar.TimeZoneDatabase','Elixir.Calendar.UTCOnlyTimeZoneDatabase','Elixir.Calendar','Elixir.CaseClauseError','Elixir.Code.Formatter','Elixir.Code.Identifier','Elixir.Code.LoadError','Elixir.Code.Typespec','Elixir.Code','Elixir.Collectable.BitString','Elixir.Collectable.File.Stream','Elixir.Collectable.HashDict','Elixir.Collectable.HashSet','Elixir.Collectable.IO.Stream','Elixir.Collectable.List','Elixir.Collectable.Map','Elixir.Collectable.MapSet','Elixir.Collectable','Elixir.CompileError','Elixir.CondClauseError','Elixir.Config.Provider','Elixir.Config.Reader','Elixir.Config','Elixir.Date.Range','Elixir.Date','Elixir.DateTime','Elixir.Dict','Elixir.DynamicSupervisor','Elixir.Enum.EmptyError','Elixir.Enum.OutOfBoundsError','Elixir.Enum','Elixir.Enumerable.Date.Range','Elixir.Enumerable.File.Stream','Elixir.Enumerable.Function','Elixir.Enumerable.GenEvent.Stream','Elixir.Enumerable.HashDict','Elixir.Enumerable.HashSet','Elixir.Enumerable.IO.Stream','Elixir.Enumerable.List','Elixir.Enumerable.Map','Elixir.Enumerable.MapSet','Elixir.Enumerable.Range','Elixir.Enumerable.Stream','Elixir.Enumerable','Elixir.ErlangError','Elixir.Exception','Elixir.File.CopyError','Elixir.File.Error','Elixir.File.LinkError','Elixir.File.RenameError','Elixir.File.Stat','Elixir.File.Stream','Elixir.File','Elixir.Float','Elixir.Function','Elixir.FunctionClauseError','Elixir.GenEvent.Stream','Elixir.GenEvent','Elixir.GenServer','Elixir.HashDict','Elixir.HashSet','Elixir.IO.ANSI.Docs','Elixir.IO.ANSI.Sequence','Elixir.IO.ANSI','Elixir.IO.Stream','Elixir.IO.StreamError','Elixir.IO','Elixir.Inspect.Algebra','Elixir.Inspect.Any','Elixir.Inspect.Atom','Elixir.Inspect.BitString','Elixir.Inspect.Date.Range','Elixir.Inspect.Date','Elixir.Inspect.DateTime','Elixir.Inspect.Error','Elixir.Inspect.Float','Elixir.Inspect.Function','Elixir.Inspect.HashDict','Elixir.Inspect.HashSet','Elixir.Inspect.Integer','Elixir.Inspect.List','Elixir.Inspect.Macro.Env','Elixir.Inspect.Map','Elixir.Inspect.MapSet','Elixir.Inspect.NaiveDateTime','Elixir.Inspect.Opts','Elixir.Inspect.PID','Elixir.Inspect.Port','Elixir.Inspect.Range','Elixir.Inspect.Reference','Elixir.Inspect.Regex','Elixir.Inspect.Stream','Elixir.Inspect.Time','Elixir.Inspect.Tuple','Elixir.Inspect.Version.Requirement','Elixir.Inspect.Version','Elixir.Inspect','Elixir.Integer','Elixir.Kernel.CLI','Elixir.Kernel.ErrorHandler','Elixir.Kernel.LexicalTracker','Elixir.Kernel.ParallelCompiler','Elixir.Kernel.ParallelRequire','Elixir.Kernel.SpecialForms','Elixir.Kernel.Typespec','Elixir.Kernel.Utils','Elixir.Kernel','Elixir.KeyError','Elixir.Keyword','Elixir.List.Chars.Atom','Elixir.List.Chars.BitString','Elixir.List.Chars.Float','Elixir.List.Chars.Integer','Elixir.List.Chars.List','Elixir.List.Chars','Elixir.List','Elixir.Macro.Env','Elixir.Macro','Elixir.Map','Elixir.MapSet','Elixir.MatchError','Elixir.Module.LocalsTracker','Elixir.Module.ParallelChecker','Elixir.Module.Types.Error','Elixir.Module.Types.Expr','Elixir.Module.Types.Helpers','Elixir.Module.Types.Of','Elixir.Module.Types.Pattern','Elixir.Module.Types.Unify','Elixir.Module.Types','Elixir.Module','Elixir.NaiveDateTime','Elixir.Node','Elixir.OptionParser.ParseError','Elixir.OptionParser','Elixir.Path.Wildcard','Elixir.Path','Elixir.Port','Elixir.Process','Elixir.Protocol.UndefinedError','Elixir.Protocol','Elixir.Range','Elixir.Record.Extractor','Elixir.Record','Elixir.Regex.CompileError','Elixir.Regex','Elixir.Registry.Partition','Elixir.Registry.Supervisor','Elixir.Registry','Elixir.RuntimeError','Elixir.Set','Elixir.Stream.Reducers','Elixir.Stream','Elixir.String.Break','Elixir.String.Casing','Elixir.String.Chars.Atom','Elixir.String.Chars.BitString','Elixir.String.Chars.Date','Elixir.String.Chars.DateTime','Elixir.String.Chars.Float','Elixir.String.Chars.Integer','Elixir.String.Chars.List','Elixir.String.Chars.NaiveDateTime','Elixir.String.Chars.Time','Elixir.String.Chars.URI','Elixir.String.Chars.Version.Requirement','Elixir.String.Chars.Version','Elixir.String.Chars','Elixir.String.Tokenizer','Elixir.String.Unicode','Elixir.String','Elixir.StringIO','Elixir.Supervisor.Default','Elixir.Supervisor.Spec','Elixir.Supervisor','Elixir.SyntaxError','Elixir.System.SignalHandler','Elixir.System','Elixir.SystemLimitError','Elixir.Task.Supervised','Elixir.Task.Supervisor','Elixir.Task','Elixir.Time','Elixir.TokenMissingError','Elixir.TryClauseError','Elixir.Tuple','Elixir.URI','Elixir.UndefinedFunctionError','Elixir.UnicodeConversionError','Elixir.Version.InvalidRequirementError','Elixir.Version.InvalidVersionError','Elixir.Version.Parser','Elixir.Version.Requirement','Elixir.Version','Elixir.WithClauseError',elixir,elixir_aliases,elixir_bitstring,elixir_bootstrap,elixir_clauses,elixir_code_server,elixir_compiler,elixir_config,elixir_def,elixir_dispatch,elixir_env,elixir_erl,elixir_erl_clauses,elixir_erl_compiler,elixir_erl_for,elixir_erl_pass,elixir_erl_try,elixir_erl_var,elixir_errors,elixir_expand,elixir_fn,elixir_import,elixir_interpolation,elixir_lexical,elixir_locals,elixir_map,elixir_module,elixir_overridable,elixir_parser,elixir_quote,elixir_rewrite,elixir_sup,elixir_tokenizer,elixir_utils],infinity,infinity},"elixir",[],"1.12.2",undefined,[],[],[kernel,stdlib,compiler]}}]
211: [{{env,kernel,shell_history_drop},[]}]
228: [{{env,logger,handle_otp_reports},true}]
237: [{{env,elixir,time_zone_database},'Elixir.Calendar.UTCOnlyTimeZoneDatabase'}]
245: [{{env,logger,translators},[{'Elixir.Logger.Translator',translate}]}]
248: [{{env,iex,colors},[]}]
255: [{{application_master,logger},<0.96.0>}]
Objects: 38
Words: 2251
Type: set
Protection: public
Compressed: false
Write Concurrency: false
Read Concurrency: true
=ets:<0.50.0>
Slot: 109377668894480
Table: #Ref<0.3590211226.1908801537.245090>
Name: code
Buckets: 443
Chain Length Avg: 1.000000
Chain Length Max: 7
Chain Length Min: 0
Chain Length Std Dev: 1.184932
Chain Length Expected Std Dev: 0.998871
Fixed: false
1: [{{sticky,v3_core},true}]
2: [{erl_prim_loader,preloaded},{supervisor,"/usr/lib/erlang/lib/stdlib-3.17/ebin/supervisor.beam"},{{sticky,io_lib_format_ryu_table},true},{erl_signal_handler,"/usr/lib/erlang/lib/kernel-8.2/ebin/erl_signal_handler.beam"},{'Elixir.GenServer',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.GenServer.beam"}]
5: [{elixir_rewrite,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_rewrite.beam"},{'Elixir.String.Unicode',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.String.Unicode.beam"}]
6: [{{sticky,gen_server},true}]
7: [{{sticky,gen_tcp},true}]
9: [{{sticky,dist_ac},true}]
10: [{{sticky,erl_error},true}]
11: [{{sticky,sys_core_fold},true}]
12: [{{sticky,random},true}]
13: [{persistent_term,preloaded}]
14: [{{sticky,raw_file_io_compressed},true}]
15: [{{sticky,disk_log_1},true}]
17: [{{sticky,beam_ssa_share},true}]
18: [{application_master,"/usr/lib/erlang/lib/kernel-8.2/ebin/application_master.beam"},{{sticky,erts_debug},true},{{sticky,global_group},true},{elixir_erl_var,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_erl_var.beam"}]
19: [{elixir_locals,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_locals.beam"}]
21: [{supervisor_bridge,"/usr/lib/erlang/lib/stdlib-3.17/ebin/supervisor_bridge.beam"}]
22: [{{sticky,raw_file_io},true}]
25: [{{sticky,io_lib_pretty},true}]
26: [{{sticky,beam_ssa_funs},true}]
28: [{net_kernel,"/usr/lib/erlang/lib/kernel-8.2/ebin/net_kernel.beam"}]
30: [{{sticky,calendar},true}]
31: [{{sticky,edlin},true}]
33: [{{sticky,beam_ssa_dead},true},{{sticky,epp},true}]
34: [{'Elixir.String.Tokenizer',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.String.Tokenizer.beam"}]
36: [{{sticky,io_lib_fread},true}]
37: [{file,"/usr/lib/erlang/lib/kernel-8.2/ebin/file.beam"},{{sticky,logger_server},true}]
38: [{'Elixir.Macro.Env',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Macro.Env.beam"}]
39: [{{sticky,seq_trace},true}]
42: [{{sticky,logger_handler_watcher},true}]
43: [{{sticky,beam_opcodes},true}]
44: [{{sticky,beam_trim},true},{{sticky,io_lib},true}]
46: [{{sticky,unicode},true}]
47: [{{sticky,proplists},true},{{sticky,code},true}]
50: [{{sticky,beam_call_types},true},{{sticky,inet6_tcp},true},{'Elixir.Code.Identifier',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Code.Identifier.beam"}]
51: [{counters,preloaded}]
53: [{{sticky,dets},true}]
59: [{{sticky,erl_compile_server},true}]
60: [{{sticky,erl_pp},true}]
63: [{{sticky,beam_peep},true},{{sticky,erl_bifs},true}]
64: [{global_group,"/usr/lib/erlang/lib/kernel-8.2/ebin/global_group.beam"}]
65: [{{sticky,beam_clean},true}]
66: [{{sticky,io},true},{{sticky,erpc},true},{standard_error,"/usr/lib/erlang/lib/kernel-8.2/ebin/standard_error.beam"},{'Elixir.IEx.Evaluator',"/usr/lib/elixir/bin/../lib/iex/ebin/Elixir.IEx.Evaluator.beam"}]
68: [{'Elixir.Inspect',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Inspect.beam"}]
69: [{{sticky,beam_flatten},true},{{sticky,dets_v9},true}]
71: [{erlang,preloaded},{string,"/usr/lib/erlang/lib/stdlib-3.17/ebin/string.beam"}]
73: [{{sticky,error_logger},true}]
76: [{{sticky,base64},true}]
77: [{{sticky,cerl_inline},true}]
79: [{{sticky,zlib},true},{{sticky,user_sup},true}]
80: [{{sticky,dist_util},true}]
82: [{{sticky,file},true},{'Elixir.String.Chars.Integer',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.String.Chars.Integer.beam"}]
84: [{'Elixir.List',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.List.beam"}]
86: [{{sticky,beam_listing},true},{user_drv,"/usr/lib/erlang/lib/kernel-8.2/ebin/user_drv.beam"}]
87: [{inet_config,"/usr/lib/erlang/lib/kernel-8.2/ebin/inet_config.beam"},{'Elixir.String',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.String.beam"}]
88: [{'Elixir.Path',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Path.beam"}]
89: [{{sticky,beam_digraph},true}]
92: [{{sticky,escript},true}]
93: [{{sticky,logger_proxy},true}]
98: [{file_io_server,"/usr/lib/erlang/lib/kernel-8.2/ebin/file_io_server.beam"}]
99: [{{sticky,binary},true},{{sticky,inet_gethost_native},true},{c,"/usr/lib/erlang/lib/stdlib-3.17/ebin/c.beam"}]
100: [{elixir_expand,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_expand.beam"}]
102: [{{sticky,slave},true}]
103: [{{sticky,beam_ssa_throw},true},{{sticky,v3_kernel},true}]
107: [{{sticky,erl_ddll},true}]
110: [{{sticky,group},true}]
112: [{prim_zip,preloaded},{{sticky,beam_ssa_opt},true},{{sticky,inet},true},{epp,"/usr/lib/erlang/lib/stdlib-3.17/ebin/epp.beam"}]
114: [{code_server,"/usr/lib/erlang/lib/kernel-8.2/ebin/code_server.beam"},{file_server,"/usr/lib/erlang/lib/kernel-8.2/ebin/file_server.beam"},{{sticky,erl_parse},true},{logger_formatter,"/usr/lib/erlang/lib/kernel-8.2/ebin/logger_formatter.beam"},{beam_lib,"/usr/lib/erlang/lib/stdlib-3.17/ebin/beam_lib.beam"}]
115: [{maps,"/usr/lib/erlang/lib/stdlib-3.17/ebin/maps.beam"},{eval_bits,"/usr/lib/erlang/lib/stdlib-3.17/ebin/eval_bits.beam"}]
116: [{{sticky,gen},true}]
118: [{{sticky,re},true}]
121: [{'Elixir.IEx.Pry',"/usr/lib/elixir/bin/../lib/iex/ebin/Elixir.IEx.Pry.beam"}]
122: [{{sticky,beam_dict},true}]
124: [{global,"/usr/lib/erlang/lib/kernel-8.2/ebin/global.beam"},{erl_internal,"/usr/lib/erlang/lib/stdlib-3.17/ebin/erl_internal.beam"}]
126: [{'Elixir.Application',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Application.beam"}]
128: [{'Elixir.Map',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Map.beam"}]
130: [{gen_server,"/usr/lib/erlang/lib/stdlib-3.17/ebin/gen_server.beam"},{'Elixir.Logger.Formatter',"/usr/lib/elixir/bin/../lib/logger/ebin/Elixir.Logger.Formatter.beam"}]
131: [{kernel_refc,"/usr/lib/erlang/lib/kernel-8.2/ebin/kernel_refc.beam"}]
132: [{{sticky,sofs},true}]
133: [{{sticky,gb_sets},true}]
134: [{{sticky,beam_ssa_pp},true},{{sticky,pool},true}]
135: [{kernel_config,"/usr/lib/erlang/lib/kernel-8.2/ebin/kernel_config.beam"}]
136: [{{sticky,erl_lint},true}]
137: [{{sticky,disk_log_server},true},{'Elixir.Kernel.CLI',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Kernel.CLI.beam"}]
139: [{{sticky,erl_distribution},true},{{sticky,kernel_config},true}]
140: [{{sticky,sys_core_alias},true}]
141: [{{sticky,auth},true}]
145: [{{sticky,proc_lib},true}]
146: [{erts_literal_area_collector,preloaded}]
147: [{{sticky,inet_tcp_dist},true}]
148: [{erl_lint,"/usr/lib/erlang/lib/stdlib-3.17/ebin/erl_lint.beam"},{heart,"/usr/lib/erlang/lib/kernel-8.2/ebin/heart.beam"},{io_lib_format,"/usr/lib/erlang/lib/stdlib-3.17/ebin/io_lib_format.beam"}]
149: [{{sticky,erl_tracer},true}]
151: [{'Elixir.IEx.Config',"/usr/lib/elixir/bin/../lib/iex/ebin/Elixir.IEx.Config.beam"}]
152: [{logger_simple_h,"/usr/lib/erlang/lib/kernel-8.2/ebin/logger_simple_h.beam"}]
153: [{binary,"/usr/lib/erlang/lib/stdlib-3.17/ebin/binary.beam"},{{sticky,sys},true},{'Elixir.IO.ANSI',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.IO.ANSI.beam"}]
157: [{{sticky,erts_literal_area_collector},true}]
159: [{{sticky,socket},true},{{sticky,inet_config},true}]
162: [{{sticky,erl_signal_handler},true},{'Elixir.IEx.Server',"/usr/lib/elixir/bin/../lib/iex/ebin/Elixir.IEx.Server.beam"},{elixir_tokenizer,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_tokenizer.beam"}]
163: [{{sticky,prim_socket},true}]
164: [{{sticky,string},true}]
165: [{{sticky,erl_reply},true}]
166: [{{sticky,file_io_server},true}]
168: [{{sticky,supervisor_bridge},true}]
169: [{{sticky,erl_init},true},{group_history,"/usr/lib/erlang/lib/kernel-8.2/ebin/group_history.beam"},{'Elixir.IEx.History',"/usr/lib/elixir/bin/../lib/iex/ebin/Elixir.IEx.History.beam"},{io_lib_pretty,"/usr/lib/erlang/lib/stdlib-3.17/ebin/io_lib_pretty.beam"}]
172: [{unicode_util,"/usr/lib/erlang/lib/stdlib-3.17/ebin/unicode_util.beam"},{'Elixir.Kernel',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Kernel.beam"}]
173: [{{sticky,logger_olp},true},{'Elixir.System',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.System.beam"}]
175: [{{sticky,beam_disasm},true},{raw_file_io,"/usr/lib/erlang/lib/kernel-8.2/ebin/raw_file_io.beam"}]
176: [{{sticky,inet_db},true},{inet_udp,"/usr/lib/erlang/lib/kernel-8.2/ebin/inet_udp.beam"}]
179: [{ets,"/usr/lib/erlang/lib/stdlib-3.17/ebin/ets.beam"},{lists,"/usr/lib/erlang/lib/stdlib-3.17/ebin/lists.beam"},{'Elixir.Access',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Access.beam"},{'Elixir.IEx.Helpers',"/usr/lib/elixir/bin/../lib/iex/ebin/Elixir.IEx.Helpers.beam"},{elixir_errors,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_errors.beam"}]
180: [{elixir_import,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_import.beam"}]
181: [{queue,"/usr/lib/erlang/lib/stdlib-3.17/ebin/queue.beam"},{{sticky,ordsets},true}]
185: [{{sticky,core_parse},true},{{sticky,logger_config},true}]
187: [{{sticky,rec_env},true}]
188: [{erl_eval,"/usr/lib/erlang/lib/stdlib-3.17/ebin/erl_eval.beam"},{kernel,"/usr/lib/erlang/lib/kernel-8.2/ebin/kernel.beam"},{{sticky,shell_docs},true},{{sticky,pg2},true},{{sticky,global_search},true}]
190: [{gen,"/usr/lib/erlang/lib/stdlib-3.17/ebin/gen.beam"},{erl_scan,"/usr/lib/erlang/lib/stdlib-3.17/ebin/erl_scan.beam"},{'Elixir.Exception',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Exception.beam"}]
192: [{group,"/usr/lib/erlang/lib/kernel-8.2/ebin/group.beam"},{elixir_sup,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_sup.beam"}]
193: [{{sticky,inet_res},true}]
194: [{logger,"/usr/lib/erlang/lib/kernel-8.2/ebin/logger.beam"},{{sticky,error_logger_tty_h},true},{timer,"/usr/lib/erlang/lib/stdlib-3.17/ebin/timer.beam"},{'Elixir.Logger.BackendSupervisor',"/usr/lib/elixir/bin/../lib/logger/ebin/Elixir.Logger.BackendSupervisor.beam"},{'Elixir.Logger.Handler',"/usr/lib/elixir/bin/../lib/logger/ebin/Elixir.Logger.Handler.beam"},{'Elixir.SyntaxError',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.SyntaxError.beam"}]
195: [{atomics,preloaded},{{sticky,prim_file},true},{{sticky,cerl},true},{{sticky,beam_ssa_pre_codegen},true},{{sticky,dict},true},{ordsets,"/usr/lib/erlang/lib/stdlib-3.17/ebin/ordsets.beam"},{'Elixir.String.Chars',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.String.Chars.beam"}]
196: [{erl_init,preloaded},{{sticky,sys_core_fold_lists},true},{{sticky,erl_expand_records},true},{{sticky,logger_filters},true},{inet,"/usr/lib/erlang/lib/kernel-8.2/ebin/inet.beam"}]
197: [{{sticky,prim_net},true},{{sticky,ets},true}]
200: [{'Elixir.IEx',"/usr/lib/elixir/bin/../lib/iex/ebin/Elixir.IEx.beam"},{'Elixir.Regex',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Regex.beam"}]
201: [{{sticky,file_sorter},true}]
202: [{{sticky,log_mf_h},true},{{sticky,qlc_pt},true}]
205: [{{sticky,logger_formatter},true}]
206: [{logger_h_common,"/usr/lib/erlang/lib/kernel-8.2/ebin/logger_h_common.beam"}]
208: [{{sticky,erl_internal},true}]
210: [{logger_server,"/usr/lib/erlang/lib/kernel-8.2/ebin/logger_server.beam"},{{sticky,maps},true},{inet_db,"/usr/lib/erlang/lib/kernel-8.2/ebin/inet_db.beam"},{'Elixir.Logger',"/usr/lib/elixir/bin/../lib/logger/ebin/Elixir.Logger.beam"},{'Elixir.Logger.Watcher',"/usr/lib/elixir/bin/../lib/logger/ebin/Elixir.Logger.Watcher.beam"}]
211: [{gb_sets,"/usr/lib/erlang/lib/stdlib-3.17/ebin/gb_sets.beam"}]
212: [{orddict,"/usr/lib/erlang/lib/stdlib-3.17/ebin/orddict.beam"}]
213: [{{sticky,socket_registry},true},{unicode,"/usr/lib/erlang/lib/stdlib-3.17/ebin/unicode.beam"},{{sticky,erl_erts_errors},true},{'Elixir.File',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.File.beam"}]
215: [{{sticky,beam_jump},true},{{sticky,cerl_clauses},true},{{sticky,net},true},{elixir_config,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_config.beam"}]
216: [{{sticky,sets},true}]
219: [{{sticky,shell_default},true}]
220: [{erts_internal,preloaded},{{sticky,beam_validator},true},{{sticky,beam_ssa_codegen},true},{{sticky,logger_h_common},true}]
221: [{'Elixir.String.Chars.Atom',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.String.Chars.Atom.beam"}]
222: [{'Elixir.IEx.Introspection',"/usr/lib/elixir/bin/../lib/iex/ebin/Elixir.IEx.Introspection.beam"}]
223: [{{sticky,kernel_refc},true},{{sticky,logger_sup},true}]
224: [{logger_olp,"/usr/lib/erlang/lib/kernel-8.2/ebin/logger_olp.beam"}]
225: [{{sticky,atomics},true}]
226: [{erl_tracer,preloaded},{erts_code_purger,preloaded},{{sticky,uri_string},true},{elixir_parser,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_parser.beam"}]
227: [{{sticky,erlang},true},{{sticky,beam_asm},true},{{sticky,orddict},true},{{sticky,shell},true},{{sticky,raw_file_io_inflate},true},{{sticky,heart},true}]
228: [{{sticky,supervisor},true}]
229: [{filename,"/usr/lib/erlang/lib/stdlib-3.17/ebin/filename.beam"},{{sticky,error_logger_file_h},true}]
230: [{{sticky,lists},true}]
231: [{logger_config,"/usr/lib/erlang/lib/kernel-8.2/ebin/logger_config.beam"},{{sticky,beam_block},true}]
232: [{{sticky,prim_zip},true}]
233: [{{sticky,erl_tar},true},{{sticky,os},true},{{sticky,wrap_log_reader},true},{{sticky,erl_boot_server},true},{'Elixir.IEx.CLI',"/usr/lib/elixir/bin/../lib/iex/ebin/Elixir.IEx.CLI.beam"}]
234: [{{sticky,v3_kernel_pp},true}]
235: [{{sticky,net_kernel},true}]
236: [{prim_eval,preloaded}]
237: [{{sticky,raw_file_io_delayed},true}]
239: [{{sticky,core_pp},true},{'Elixir.IO',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.IO.beam"}]
241: [{{sticky,code_server},true},{'Elixir.Inspect.Algebra',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Inspect.Algebra.beam"}]
242: [{zlib,preloaded},{prim_buffer,preloaded},{error_handler,"/usr/lib/erlang/lib/kernel-8.2/ebin/error_handler.beam"},{{sticky,disk_log},true},{io_lib,"/usr/lib/erlang/lib/stdlib-3.17/ebin/io_lib.beam"},{'Elixir.Supervisor',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Supervisor.beam"}]
243: [{logger_filters,"/usr/lib/erlang/lib/kernel-8.2/ebin/logger_filters.beam"}]
244: [{prim_socket,preloaded},{{sticky,raw_file_io_deflate},true}]
245: [{{sticky,prim_inet},true},{{sticky,error_handler},true}]
246: [{{sticky,erl_abstract_code},true},{{sticky,inet_sctp},true}]
247: [{{sticky,inet6_udp},true}]
248: [{{sticky,application_starter},true}]
253: [{{sticky,erl_prim_loader},true},{{sticky,prim_eval},true},{{sticky,application_master},true},{'Elixir.Inspect.Atom',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Inspect.Atom.beam"}]
254: [{{sticky,beam_ssa_lint},true},{{sticky,qlc},true},{erl_distribution,"/usr/lib/erlang/lib/kernel-8.2/ebin/erl_distribution.beam"},{edlin,"/usr/lib/erlang/lib/stdlib-3.17/ebin/edlin.beam"}]
255: [{{sticky,gen_event},true},{io,"/usr/lib/erlang/lib/stdlib-3.17/ebin/io.beam"}]
256: [{user_sup,"/usr/lib/erlang/lib/kernel-8.2/ebin/user_sup.beam"}]
258: [{application_controller,"/usr/lib/erlang/lib/kernel-8.2/ebin/application_controller.beam"},{elixir,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir.beam"},{'Elixir.Logger.Filter',"/usr/lib/elixir/bin/../lib/logger/ebin/Elixir.Logger.Filter.beam"}]
259: [{{sticky,beam_ssa_type},true},{{sticky,otp_internal},true}]
260: [{init,preloaded},{{sticky,gen_tcp_socket},true}]
261: [{erl_parse,"/usr/lib/erlang/lib/stdlib-3.17/ebin/erl_parse.beam"}]
262: [{{sticky,rand},true}]
264: [{{sticky,erts_internal},true}]
267: [{{sticky,gen_fsm},true}]
269: [{{sticky,global},true}]
271: [{{sticky,kernel},true}]
272: [{{sticky,beam_ssa_recv},true},{logger_sup,"/usr/lib/erlang/lib/kernel-8.2/ebin/logger_sup.beam"}]
274: [{logger_handler_watcher,"/usr/lib/erlang/lib/kernel-8.2/ebin/logger_handler_watcher.beam"}]
275: [{gb_trees,"/usr/lib/erlang/lib/stdlib-3.17/ebin/gb_trees.beam"},{'Elixir.Inspect.Opts',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Inspect.Opts.beam"}]
277: [{{sticky,beam_types},true}]
279: [{{sticky,beam_ssa_bool},true}]
280: [{{sticky,sys_core_inline},true}]
284: [{{sticky,beam_kernel_to_ssa},true}]
287: [{{sticky,sys_pre_attributes},true}]
288: [{{sticky,logger_std_h},true}]
289: [{{sticky,digraph},true},{{sticky,io_lib_format},true}]
291: [{proplists,"/usr/lib/erlang/lib/stdlib-3.17/ebin/proplists.beam"}]
292: [{logger_backend,"/usr/lib/erlang/lib/kernel-8.2/ebin/logger_backend.beam"},{{sticky,gen_sctp},true}]
293: [{{sticky,sys_messages},true},{{sticky,c},true},{{sticky,logger},true}]
297: [{{sticky,ms_transform},true}]
299: [{'Elixir.String.Break',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.String.Break.beam"}]
300: [{{sticky,dets_server},true}]
301: [{{sticky,inet_udp},true}]
302: [{{sticky,beam_z},true}]
304: [{{sticky,beam_a},true},{{sticky,edlin_expand},true}]
305: [{{sticky,inet_dns},true}]
307: [{elixir_utils,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_utils.beam"}]
308: [{{sticky,inet_hosts},true}]
309: [{{sticky,prim_buffer},true}]
311: [{{sticky,raw_file_io_list},true},{'Elixir.Logger.Config',"/usr/lib/elixir/bin/../lib/logger/ebin/Elixir.Logger.Config.beam"}]
312: [{elixir_dispatch,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_dispatch.beam"}]
313: [{{sticky,init},true},{logger_proxy,"/usr/lib/erlang/lib/kernel-8.2/ebin/logger_proxy.beam"},{{sticky,win32reg},true}]
315: [{{sticky,erl_epmd},true}]
318: [{{sticky,core_scan},true},{{sticky,erl_posix_msg},true}]
319: [{{sticky,disk_log_sup},true}]
322: [{error_logger,"/usr/lib/erlang/lib/kernel-8.2/ebin/error_logger.beam"},{'Elixir.Agent.Server',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Agent.Server.beam"}]
323: [{{sticky,queue},true}]
324: [{{sticky,math},true},{{sticky,beam_lib},true}]
326: [{{sticky,beam_ssa},true}]
328: [{{sticky,filelib},true}]
329: [{socket_registry,preloaded}]
333: [{'Elixir.Enum',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Enum.beam"}]
336: [{'Elixir.Logger.App',"/usr/lib/elixir/bin/../lib/logger/ebin/Elixir.Logger.App.beam"}]
338: [{erts_dirty_process_signal_handler,preloaded}]
339: [{'Elixir.Process',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Process.beam"},{elixir_aliases,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_aliases.beam"},{elixir_erl_pass,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_erl_pass.beam"}]
340: [{prim_inet,preloaded},{'Elixir.Agent',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Agent.beam"}]
341: [{inet_parse,"/usr/lib/erlang/lib/kernel-8.2/ebin/inet_parse.beam"},{'Elixir.Logger.Backends.Console',"/usr/lib/elixir/bin/../lib/logger/ebin/Elixir.Logger.Backends.Console.beam"},{'Elixir.Node',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Node.beam"},{'Elixir.Code',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Code.beam"}]
342: [{elixir_env,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_env.beam"}]
344: [{{sticky,dets_sup},true},{{sticky,timer},true}]
346: [{{sticky,application},true}]
354: [{{sticky,eval_bits},true}]
355: [{os,"/usr/lib/erlang/lib/kernel-8.2/ebin/os.beam"},{{sticky,erl_anno},true},{rpc,"/usr/lib/erlang/lib/kernel-8.2/ebin/rpc.beam"}]
357: [{{sticky,standard_error},true}]
358: [{{sticky,inet6_sctp},true}]
360: [{{sticky,core_lib},true}]
363: [{{sticky,rpc},true}]
368: [{{sticky,sys_core_prepare},true}]
369: [{{sticky,pg},true}]
370: [{elixir_code_server,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_code_server.beam"}]
371: [{{sticky,local_udp},true}]
372: [{{sticky,gen_statem},true},{'Elixir.Keyword',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Keyword.beam"}]
374: [{{sticky,dets_utils},true}]
376: [{{sticky,inet6_tcp_dist},true}]
379: [{{sticky,counters},true},{{sticky,user},true},{{sticky,ram_file},true}]
380: [{{sticky,erts_code_purger},true}]
382: [{application,"/usr/lib/erlang/lib/kernel-8.2/ebin/application.beam"}]
386: [{proc_lib,"/usr/lib/erlang/lib/stdlib-3.17/ebin/proc_lib.beam"},{{sticky,filename},true}]
387: [{'Elixir.IO.ANSI.Docs',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.IO.ANSI.Docs.beam"}]
389: [{inet_gethost_native,"/usr/lib/erlang/lib/kernel-8.2/ebin/inet_gethost_native.beam"},{re,"/usr/lib/erlang/lib/stdlib-3.17/ebin/re.beam"}]
390: [{{sticky,logger_backend},true}]
393: [{{sticky,core_lint},true}]
394: [{{sticky,erl_stdlib_errors},true}]
395: [{{sticky,file_server},true}]
396: [{elixir_erl,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_erl.beam"}]
397: [{{sticky,unicode_util},true},{{sticky,user_drv},true}]
399: [{erl_anno,"/usr/lib/erlang/lib/stdlib-3.17/ebin/erl_anno.beam"}]
400: [{'Elixir.IEx.App',"/usr/lib/elixir/bin/../lib/iex/ebin/Elixir.IEx.App.beam"}]
402: [{'Elixir.CompileError',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.CompileError.beam"}]
404: [{gen_event,"/usr/lib/erlang/lib/stdlib-3.17/ebin/gen_event.beam"},{'Elixir.Supervisor.Default',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Supervisor.Default.beam"}]
405: [{{sticky,inet_parse},true}]
406: [{{sticky,persistent_term},true}]
407: [{{sticky,logger_simple_h},true}]
408: [{logger_std_h,"/usr/lib/erlang/lib/kernel-8.2/ebin/logger_std_h.beam"}]
413: [{{sticky,cerl_trees},true},{{sticky,zip},true}]
415: [{{sticky,logger_disk_log_h},true}]
416: [{{sticky,gen_udp},true}]
417: [{{sticky,digraph_utils},true}]
418: [{{sticky,array},true},{'Elixir.IEx.Broker',"/usr/lib/elixir/bin/../lib/iex/ebin/Elixir.IEx.Broker.beam"}]
419: [{{sticky,erts_dirty_process_signal_handler},true},{{sticky,erl_kernel_errors},true}]
421: [{code,"/usr/lib/erlang/lib/kernel-8.2/ebin/code.beam"},{{sticky,gen_udp_socket},true},{{sticky,group_history},true},{elixir_quote,"/usr/lib/elixir/bin/../lib/elixir/ebin/elixir_quote.beam"}]
427: [{{sticky,inet_tcp},true}]
428: [{{sticky,erl_eval},true},{{sticky,application_controller},true}]
432: [{{sticky,erl_compile},true},{{sticky,erl_bits},true}]
433: [{{sticky,beam_ssa_bsm},true}]
434: [{'Elixir.Inspect.Integer',"/usr/lib/elixir/bin/../lib/elixir/ebin/Elixir.Inspect.Integer.beam"}]
435: [{{sticky,sys_core_bsm},true}]
436: [{prim_net,preloaded},{{sticky,erl_scan},true},{{sticky,local_tcp},true}]
437: [{prim_file,preloaded},{{sticky,gb_trees},true}]
438: [{{sticky,beam_utils},true}]
439: [{{sticky,compile},true},{{sticky,net_adm},true}]
442: [{{sticky,beam_ssa_bc_size},true}]
Objects: 443
Words: 24382
Type: set
Protection: private
Compressed: false
Write Concurrency: false
Read Concurrency: false
=ets:<0.50.0>
Slot: 123385461221752
Table: code_names
Name: code_names
Buckets: 256
Chain Length Avg: 0.097656
Chain Length Max: 1
Chain Length Min: 0
Chain Length Std Dev: 0.296849
Chain Length Expected Std Dev: 0.311889
Fixed: false
10: [{"tftp","/usr/lib/erlang/lib/tftp-1.0.3","tftp-1.0.3",[]}]
19: [{"stdlib","/usr/lib/erlang/lib/stdlib-3.17","stdlib-3.17",[]}]
26: [{"ssl","/usr/lib/erlang/lib/ssl-10.6.1","ssl-10.6.1",[]}]
30: [{"public_key","/usr/lib/erlang/lib/public_key-1.11.3","public_key-1.11.3",[]}]
38: [{"iex","/usr/lib/elixir/bin/../lib/iex","iex",[]}]
57: [{"ftp","/usr/lib/erlang/lib/ftp-1.1","ftp-1.1",[]}]
61: [{"eex","/usr/lib/elixir/bin/../lib/eex","eex",[]}]
93: [{"sasl","/usr/lib/erlang/lib/sasl-4.1.1","sasl-4.1.1",[]}]
99: [{".",".",".",[]}]
106: [{"parsetools","/usr/lib/erlang/lib/parsetools-2.3.2","parsetools-2.3.2",[]}]
124: [{"runtime_tools","/usr/lib/erlang/lib/runtime_tools-1.17","runtime_tools-1.17",[]}]
126: [{"compiler","/usr/lib/erlang/lib/compiler-8.0.4","compiler-8.0.4",[]}]
127: [{"asn1","/usr/lib/erlang/lib/asn1-5.0.17","asn1-5.0.17",[]}]
130: [{"inets","/usr/lib/erlang/lib/inets-7.5","inets-7.5",[]}]
143: [{"tools","/usr/lib/erlang/lib/tools-3.5.2","tools-3.5.2",[]}]
152: [{"erl_interface","/usr/lib/erlang/lib/erl_interface-5.1","erl_interface-5.1",[]}]
154: [{"erts","/usr/lib/erlang/lib/erts-12.2.1","erts-12.2.1",[]}]
155: [{"crypto","/usr/lib/erlang/lib/crypto-5.0.5","crypto-5.0.5",[]}]
161: [{"elixir","/usr/lib/elixir/bin/../lib/elixir","elixir",[]}]
175: [{"logger","/usr/lib/elixir/bin/../lib/logger","logger",[]}]
203: [{"kernel","/usr/lib/erlang/lib/kernel-8.2","kernel-8.2",[]}]
221: [{"mix","/usr/lib/elixir/bin/../lib/mix","mix",[]}]
222: [{"mnesia","/usr/lib/erlang/lib/mnesia-4.20.1","mnesia-4.20.1",[]}]
225: [{"ex_unit","/usr/lib/elixir/bin/../lib/ex_unit","ex_unit",[]}]
227: [{"syntax_tools","/usr/lib/erlang/lib/syntax_tools-2.6","syntax_tools-2.6",[]}]
Objects: 25
Words: 2884
Type: set
Protection: public
Compressed: false
Write Concurrency: false
Read Concurrency: false
=ets:<0.51.0>
Slot: 123385461285096
Table: inet_db
Name: inet_db
Buckets: 256
Chain Length Avg: 0.117188
Chain Length Max: 3
Chain Length Min: 0
Chain Length Std Dev: 0.356219
Chain Length Expected Std Dev: 0.341657
Fixed: false
3: [{res_usevc,false}]
5: [{res_hosts_file,"/etc/hosts"}]
8: [{res_search,[]}]
34: [{socks5_server,[]}]
63: [{res_hosts_file_info,undefined}]
69: [{tcp_module,inet_tcp},{udp_module,inet_udp},{sctp_module,inet_sctp}]
79: [{res_resolv_conf_info,undefined}]
80: [{res_lookup,[native]}]
83: [{res_ns,[]}]
89: [{res_retry,3}]
110: [{res_domain,[]}]
125: [{res_resolv_conf_tm,-576460758}]
149: [{cache_size,100}]
164: [{res_timeout,2000}]
173: [{res_hosts_file_tm,-576460758}]
179: [{socks5_methods,[none]}]
180: [{socks5_port,1080}]
181: [{res_udp_payload_size,1280}]
182: [{res_inet6,false}]
188: [{cache_refresh_interval,3600000}]
195: [{res_alt_ns,[]}]
197: [{hostname,"fer-VivoBook-ASUSLaptop-X509DA-M509DA"}]
211: [{res_edns,false}]
212: [{res_servfail_retry_timeout,1500}]
230: [{res_resolv_conf,"/etc/resolv.conf"}]
244: [{res_id,0}]
245: [{res_recurse,true}]
249: [{socks5_noproxy,[]}]
Objects: 30
Words: 645
Type: set
Protection: public
Compressed: false
Write Concurrency: false
Read Concurrency: false
=ets:<0.51.0>
Slot: 123385461289040
Table: inet_cache
Name: inet_cache
Buckets: 256
Chain Length Avg: 0.000000
Chain Length Max: 0
Chain Length Min: 0
Chain Length Std Dev: 0.000000
Chain Length Expected Std Dev: 0.000000
Fixed: false
Objects: 0
Words: 305
Type: bag
Protection: public
Compressed: false
Write Concurrency: false
Read Concurrency: false
=ets:<0.51.0>
Slot: 123385461291496
Table: inet_hosts_byname
Name: inet_hosts_byname
Buckets: 256
Chain Length Avg: 0.000000
Chain Length Max: 0
Chain Length Min: 0
Chain Length Std Dev: 0.000000
Chain Length Expected Std Dev: 0.000000
Fixed: false
Objects: 0
Words: 305
Type: set
Protection: protected
Compressed: false
Write Concurrency: false
Read Concurrency: false
=ets:<0.51.0>
Slot: 123385461293952
Table: inet_hosts_byaddr
Name: inet_hosts_byaddr
Buckets: 256
Chain Length Avg: 0.000000
Chain Length Max: 0
Chain Length Min: 0
Chain Length Std Dev: 0.000000
Chain Length Expected Std Dev: 0.000000
Fixed: false
Objects: 0
Words: 305
Type: set
Protection: protected
Compressed: false
Write Concurrency: false
Read Concurrency: false
=ets:<0.51.0>
Slot: 123385461296408
Table: inet_hosts_file_byname
Name: inet_hosts_file_byname
Buckets: 256
Chain Length Avg: 0.000000
Chain Length Max: 0
Chain Length Min: 0
Chain Length Std Dev: 0.000000
Chain Length Expected Std Dev: 0.000000
Fixed: false
Objects: 0
Words: 305
Type: set
Protection: protected
Compressed: false
Write Concurrency: false
Read Concurrency: false
=ets:<0.51.0>
Slot: 123385461298864
Table: inet_hosts_file_byaddr
Name: inet_hosts_file_byaddr
Buckets: 256
Chain Length Avg: 0.000000
Chain Length Max: 0
Chain Length Min: 0
Chain Length Std Dev: 0.000000
Chain Length Expected Std Dev: 0.000000
Fixed: false
Objects: 0
Words: 305
Type: set
Protection: protected
Compressed: false
Write Concurrency: false
Read Concurrency: false
=ets:<0.51.0>
Slot: 123385461301320
Table: inet_sockets
Name: inet_sockets
Buckets: 256
Chain Length Avg: 0.000000
Chain Length Max: 0
Chain Length Min: 0
Chain Length Std Dev: 0.000000
Chain Length Expected Std Dev: 0.000000
Fixed: false
Objects: 0
Words: 305
Type: set
Protection: protected
Compressed: false
Write Concurrency: false
Read Concurrency: false
=ets:<0.54.0>
Slot: 123385461310368
Table: #Ref<0.3590211226.1908801537.245131>
Name: rex_nodes_observer
Buckets: 256
Chain Length Avg: 0.000000
Chain Length Max: 0
Chain Length Min: 0
Chain Length Std Dev: 0.000000
Chain Length Expected Std Dev: 0.000000
Fixed: false
Objects: 0
Words: 305
Type: set
Protection: protected
Compressed: false
Write Concurrency: false
Read Concurrency: true
=ets:<0.55.0>
Slot: 123385461313640
Table: global_locks
Name: global_locks
Buckets: 256
Chain Length Avg: 0.000000
Chain Length Max: 0
Chain Length Min: 0
Chain Length Std Dev: 0.000000
Chain Length Expected Std Dev: 0.000000
Fixed: false
Objects: 0
Words: 305
Type: set
Protection: protected
Compressed: false
Write Concurrency: false
Read Concurrency: false
=ets:<0.55.0>
Slot: 123385461316096
Table: global_names
Name: global_names
Buckets: 256
Chain Length Avg: 0.000000
Chain Length Max: 0
Chain Length Min: 0
Chain Length Std Dev: 0.000000
Chain Length Expected Std Dev: 0.000000
Fixed: false
Objects: 0
Words: 305
Type: set
Protection: protected
Compressed: false
Write Concurrency: false
Read Concurrency: true
=ets:<0.55.0>
Slot: 123385461318552
Table: global_names_ext
Name: global_names_ext
Buckets: 256
Chain Length Avg: 0.000000
Chain Length Max: 0
Chain Length Min: 0
Chain Length Std Dev: 0.000000
Chain Length Expected Std Dev: 0.000000
Fixed: false
Objects: 0
Words: 305
Type: set
Protection: protected
Compressed: false
Write Concurrency: false
Read Concurrency: false
=ets:<0.55.0>
Slot: 123385461321008
Table: global_pid_names
Name: global_pid_names
Buckets: 256
Chain Length Avg: 0.000000
Chain Length Max: 0
Chain Length Min: 0
Chain Length Std Dev: 0.000000
Chain Length Expected Std Dev: 0.000000
Fixed: false
Objects: 0
Words: 305
Type: bag
Protection: protected
Compressed: false
Write Concurrency: false
Read Concurrency: false
=ets:<0.55.0>
Slot: 123385461323464
Table: global_pid_ids
Name: global_pid_ids
Buckets: 256
Chain Length Avg: 0.000000
Chain Length Max: 0
Chain Length Min: 0
Chain Length Std Dev: 0.000000
Chain Length Expected Std Dev: 0.000000
Fixed: false
Objects: 0
Words: 305
Type: bag
Protection: protected
Compressed: false
Write Concurrency: false
Read Concurrency: false
=ets:<0.59.0>
Slot: 123385461328688
Table: file_io_servers
Name: file_io_servers
Buckets: 256
Chain Length Avg: 0.000000
Chain Length Max: 0
Chain Length Min: 0
Chain Length Std Dev: 0.000000
Chain Length Expected Std Dev: 0.000000
Fixed: false
Objects: 0
Words: 305
Type: set
Protection: protected
Compressed: false
Write Concurrency: false
Read Concurrency: false
=ets:<0.83.0>
Slot: 123385461373976
Table: elixir_config
Name: elixir_config
Buckets: 256
Chain Length Avg: 0.074219
Chain Length Max: 1
Chain Length Min: 0
Chain Length Std Dev: 0.262127
Chain Length Expected Std Dev: 0.271899
Fixed: false
3: [{warnings_as_errors,false}]
4: [{ignore_module_conflict,false}]
19: [{parser_options,[]}]
36: [{no_warn_undefined,[]}]
68: [{no_halt,true}]
95: [{debug_info,true}]
100: [{at_exit,[]}]
149: [{{uri,<<"https">>},443}]
152: [{{uri,<<"tftp">>},69}]
163: [{docs,true}]
171: [{{uri,<<"sftp">>},22}]
178: [{identifier_tokenizer,'Elixir.String.Tokenizer'}]
179: [{relative_paths,true}]
184: [{{uri,<<"ldap">>},389}]
185: [{{uri,<<"http">>},80}]
197: [{{uri,<<"ftp">>},21}]
224: [{bootstrap,false}]
227: [{tracers,[]}]
230: [{argv,[]}]
Objects: 19
Words: 474
Type: set
Protection: public
Compressed: false
Write Concurrency: false
Read Concurrency: true
=ets:<0.86.0>
Slot: 123385461379920
Table: elixir_modules
Name: elixir_modules
Buckets: 256
Chain Length Avg: 0.000000
Chain Length Max: 0
Chain Length Min: 0
Chain Length Std Dev: 0.000000
Chain Length Expected Std Dev: 0.000000
Fixed: false
Objects: 0
Words: 305
Type: set
Protection: public
Compressed: false
Write Concurrency: false
Read Concurrency: true
=ets:<0.91.0>
Slot: 123385461395504
Table: 'Elixir.IEx.Config'
Name: 'Elixir.IEx.Config'
Buckets: 256
Chain Length Avg: 0.003906
Chain Length Max: 1
Chain Length Min: 0
Chain Length Std Dev: 0.062378
Chain Length Expected Std Dev: 0.062378
Fixed: false
30: [{after_spawn,[]}]
Objects: 1
Words: 312
Type: set
Protection: public
Compressed: false
Write Concurrency: false
Read Concurrency: false
=ets:<0.93.0>
Slot: 123385461398024
Table: 'Elixir.IEx.Pry'
Name: 'Elixir.IEx.Pry'
Buckets: 256
Chain Length Avg: 0.000000
Chain Length Max: 0
Chain Length Min: 0
Chain Length Std Dev: 0.000000
Chain Length Expected Std Dev: 0.000000
Fixed: false
Objects: 0
Words: 1329
Type: set
Protection: public
Compressed: false
Write Concurrency: true
Read Concurrency: false

--------------------------------------------------------------------------------------------------


iex(3)> 
BREAK: (a)bort (A)bort with dump (c)ontinue (p)roc info (i)nfo
       (l)oaded (v)ersion (k)ill (D)b-tables (d)istribution
k


Process Information

--------------------------------------------------
=proc:<0.889.0>
State: Waiting
Spawned as: erlang:apply/2
Spawned by: <0.74.0>
Message queue length: 0
Number of heap fragments: 1
Heap fragment data: 14
Link list: [{to,<0.66.0>,#Ref<0.1991307518.1642594305.188446>}]
Reductions: 4023
Stack+heap: 233
OldHeap: 0
Heap unused: 111
OldHeap unused: 0
BinVHeap: 3
OldBinVHeap: 0
BinVHeap unused: 46419
OldBinVHeap unused: 46422
Memory: 2784
Stack dump:
Program counter: 0x00007e77a7c54ea0 (io:execute_request/3 + 360)
arity = 0
y(0)     #Ref<0.1991307518.1642594305.188446>
y(1)     error
y(2)     {false,{get_line,unicode,<<"iex(3)> ">>}}
y(3)     <0.66.0>

0x00007e77a48e88f8 Return addr 0x00007e77a7cd9efc ('Elixir.IEx.Server':io_get/4 + 148)
y(0)     <0.889.0>
y(1)     <0.74.0>

0x00007e77a48e8910 Return addr 0x00007e77a7800948 (<terminate process normally>)

0x00007e77a48e8918 Return addr 0x00007e77a7800948 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
(k)ill (n)ext (r)eturn:
n
=proc:<0.106.0>
State: Waiting
Spawned as: proc_lib:init_p/5
Spawned by: <0.74.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [{from,<0.74.0>,#Ref<0.1991307518.1642594307.182411>}]
Dictionary: [{'$initial_call',{'Elixir.IEx.Evaluator',init,4}},{'$ancestors',[<0.74.0>]},{iex_server,<0.74.0>},{iex_evaluator,#Ref<0.1991307518.1642594307.182376>}]
Reductions: 3765897
Stack+heap: 4185
OldHeap: 4185
Heap unused: 3326
OldHeap unused: 1943
BinVHeap: 3
OldBinVHeap: 49
BinVHeap unused: 46419
OldBinVHeap unused: 46373
Memory: 67872
Stack dump:
Program counter: 0x00007e77a7d2b53c ('Elixir.IEx.Evaluator':loop/1 + 148)
arity = 0
y(0)     #Ref<0.1991307518.1642594307.182376>
y(1)     <0.74.0>
y(2)     #{binding=>[],env=>#{'__struct__'=>'Elixir.Macro.Env',aliases=>[],context=>nil,context_modules=>[],contextual_vars=>[],current_vars=>{#{},false},file=><<"iex">>,function=>nil,functions=>[{'Elixir.IEx.Helpers',[{'break!',3},{'break!',4},{breaks,0},{c,1},{c,2},{cd,1},{clear,0},{continue,0},{exports,0},{exports,1},{flush,0},{h,0},{i,0},{i,1},{l,1},{ls,0},{ls,1},{nl,1},{nl,2},{open,0},{pid,1},{pid,3},{port,1},{port,2},{pwd,0},{r,1},{recompile,0},{recompile,1},{ref,1},{ref,4},{remove_breaks,0},{remove_breaks,1},{reset_break,1},{reset_break,3},{respawn,0},{runtime_info,0},{runtime_info,1},{v,0},{v,1},{whereami,0},{whereami,1}]},{'Elixir.Kernel',[{'!=',2},{'!==',2},{'*',2},{'+',1},{'+',2},{'++',2},{'-',1},{'-',2},{'--',2},{'/',2},{'<',2},{'<=',2},{'==',2},{'===',2},{'=~',2},{'>',2},{'>=',2},{abs,1},{apply,2},{apply,3},{binary_part,3},{bit_size,1},{byte_size,1},{ceil,1},{div,2},{elem,2},{exit,1},{floor,1},{'function_exported?',3},{get_and_update_in,3},{get_in,2},{hd,1},{inspect,1},{inspect,2},{is_atom,1},{is_binary,1},{is_bitstring,1},{is_boolean,1},{is_float,1},{is_function,1},{is_function,2},{is_integer,1},{is_list,1},{is_map,1},{is_map_key,2},{is_number,1},{is_pid,1},{is_port,1},{is_reference,1},{is_tuple,1},{length,1},{'macro_exported?',3},{make_ref,0},{map_size,1},{max,2},{min,2},{node,0},{node,1},{not,1},{pop_in,2},{put_elem,3},{put_in,3},{rem,2},{round,1},{self,0},{send,2},{spawn,1},{spawn,3},{spawn_link,1},{spawn_link,3},{spawn_monitor,1},{spawn_monitor,3},{struct,1},{struct,2},{'struct!',1},{'struct!',2},{throw,1},{tl,1},{trunc,1},{tuple_size,1},{update_in,3}]}],lexical_tracker=>nil,line=>1,macro_aliases=>[],macros=>[{'Elixir.IEx.Helpers',[{b,1},{'break!',1},{'break!',2},{h,1},{import_file,1},{import_file,2},{import_file_if_available,1},{import_if_available,1},{import_if_available,2},{open,1},{t,1},{use_if_available,1},{use_if_available,2}]},{'Elixir.Kernel',[{'!',1},{'&&',2},{'..',2},{'..//',3},{'<>',2},{'@',1},{'alias!',1},{and,2},{binding,0},{binding,1},{def,1},{def,2},{defdelegate,2},{defexception,1},{defguard,1},{defguardp,1},{defimpl,2},{defimpl,3},{defmacro,1},{defmacro,2},{defmacrop,1},{defmacrop,2},{defmodule,2},{defoverridable,1},{defp,1},{defp,2},{defprotocol,2},{defstruct,1},{destructure,2},{get_and_update_in,2},{if,2},{in,2},{is_exception,1},{is_exception,2},{is_nil,1},{is_struct,1},{is_struct,2},{'match?',2},{or,2},{pop_in,1},{put_in,2},{raise,1},{raise,2},{reraise,2},{reraise,3},{sigil_C,2},{sigil_D,2},{sigil_N,2},{sigil_R,2},{sigil_S,2},{sigil_T,2},{sigil_U,2},{sigil_W,2},{sigil_c,2},{sigil_r,2},{sigil_s,2},{sigil_w,2},{tap,2},{then,2},{to_char_list,1},{to_charlist,1},{to_string,1},{unless,2},{update_in,2},{use,1},{use,2},{'var!',1},{'var!',2},{'|>',2},{'||',2}]}],module=>nil,prematch_vars=>apply,requires=>['Elixir.Application','Elixir.IEx.Helpers','Elixir.Kernel','Elixir.Kernel.Typespec'],tracers=>[],unused_vars=>{#{},0},vars=>[]},history=>#{'__struct__'=>'Elixir.IEx.History',queue=>{[{2,nil}],[{1,'Elixir.D'}]},size=>2,start=>1},ref=>#Ref<0.1991307518.1642594307.182376>,server=><0.74.0>,stacktrace=>nil}

0x00007e77a48f9a18 Return addr 0x00007e77a7d2b144 ('Elixir.IEx.Evaluator':init/4 + 652)
y(0)     nil
y(1)     nil
y(2)     []
y(3)     []
y(4)     <0.66.0>
y(5)     []
y(6)     Catch 0x00007e77a7d2b19f ('Elixir.IEx.Evaluator':init/4 + 743)

0x00007e77a48f9a58 Return addr 0x00007e77a7955e14 (proc_lib:init_p_do_apply/3 + 196)
y(0)     []
y(1)     []
y(2)     Catch 0x00007e77a7955e34 (proc_lib:init_p_do_apply/3 + 228)

0x00007e77a48f9a78 Return addr 0x00007e77a7800948 (<terminate process normally>)

0x00007e77a48f9a80 Return addr 0x00007e77a7800948 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
(k)ill (n)ext (r)eturn:


-----------------------------------------------------------------------------------------------------------------




