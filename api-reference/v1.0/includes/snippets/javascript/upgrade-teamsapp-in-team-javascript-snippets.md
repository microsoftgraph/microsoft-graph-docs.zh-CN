---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9faab5402439488e2133963e530331ae74bfa98309d8a640a5933b6d1031fc64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333739"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/db5e04be-daa2-4a35-beb1-5e73cc381599/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=/upgrade')
    .post();

```