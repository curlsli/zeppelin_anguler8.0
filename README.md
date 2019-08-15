git clone http://git.code.oa.com/vcms/cctv-tim.git;

基础设置

```yaml
  152.136.47.44 auth.cctvtest.com
  127.0.0.1 tt.cctvtest.com
```
  node 12+
  
run:

```bash
  cd cctv-tim 
  npm i
  npm run start
```
方案1：

    home.component.ts的auth.*的接口，需要业务接口统一替代，否则有跨域问题

方案2：

    设置域名白名单，用统一的auth.test允许跨域，来统一返回请求结果
