# Jira Release 발생시 Slack에 Release Notes 발행하기


![app1](./images/app1.png)

![app2](./images/app2.png)

![app3](./images/app3.png)

![app4](./images/app4.png)

![app5](./images/app5.png)

![app6](./images/app6.png)

![app7](./images/app7.png)

![app8](./images/app8.png)

![app9](./images/app9.png)

![app10](./images/app10.png)



```bash
project = 프로젝트ID AND fixVersion = '{{version.name}}'
```

```bash
시스템이 운영 배포 되었습니다. 

version: {{version.name}}
releasedAt: {{now.jqlDateTime.convertToTimeZone("Asia/Seoul")}}

-------- 반영 티켓 --------

{{#lookupIssues}}
- <{{url}}|[{{key}}]> {{summary}}
{{/}}
```

* https://support.atlassian.com/cloud-automation/docs/what-are-smart-values/

## 최종


![release1](./images/release1.png)

![release2](./images/release2.png)

![result](./images/result.png)
