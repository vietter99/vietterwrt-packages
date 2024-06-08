## Getting started

### Build project

```bash
git clone --depth 1 --branch master --single-branch --no-checkout https://github.com/vietter99/luci-theme-argon.git package/luci-theme-argon
pushd package/luci-theme-argon
umask 022
git checkout
popd
```

### Build for OpenWrt official SnapShots and ImmortalWrt

```bash
echo "src-git modemfeed https://github.com/vietter99/luci-theme-argon.git" >> "feeds.conf.default"
make menuconfig #choose LUCI->Theme->Luci-theme-argon
make -j1 V=s
```
## Wanted

## Notice

- Chrome browser is highly recommended. There are some new css3 features used in this theme, currently only Chrome has the best compatibility.
- Currently, the mainline version of the IE series has bugs that need to be addressed.
- FireFox does not enable the backdrop-filter by default, [see here](https://developer.mozilla.org/zh-CN/docs/Web/CSS/backdrop-filter) for the opening method.
