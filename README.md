# mTCP
mTCP for newer DPDK version (~23.11)

# Build
Make sure you have built DPDK library and pkg-config successfully recognize libdpdk. Current version uses DPDK 23.11. After building DPDK, you should check PMD for your NIC. If you are using Mellanox NIC, you don't need to explicitly bind PMD. Or, you might need to unbind the kernel driver to re-bind PMD.
After checking your NIC using testpmd application, go to mTCP src directory and just make it.

```Bash
cd src
make -j
```

Now you will have src/lib/libmtcp.a.

