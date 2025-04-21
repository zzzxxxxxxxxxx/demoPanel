# demoPanel

混淆个人专属 BPB 代码。详细搭建过程参见 [demoPanel](https://www.haoyep.com/posts/cf-bpb-vpn/)。

BPB在[Release v3.2.3](https://github.com/bia-pain-bache/BPB-Worker-Panel/releases/tag/v3.2.3)中指出，直接未经混淆的代码很容易让Cloudflare检测到并报1101错误。因此本文不再更新混淆脚本。实际上，已经成功部署的BPB脚本也一直是可以正常运行的，没必要跟进最新版本。如果确实想自己混淆，可以拉BPB库，按照[workflows](https://github.com/bia-pain-bache/BPB-Worker-Panel/blob/main/.github/workflows/build.yml)过程编译混淆。
>1- None obfuscated files removed from releases forever, due to code exposures to Cloudflare (possible 1101 errors in future). So please choose a Cloudflare account which haven't returned 1101 before.
2- If you are using Workers deployment and got 1101, please delete the worker and change subdomain from Workers & Pages > Subdomain from right hand toolbar. It will take a few minutes to apply new subdomain.
