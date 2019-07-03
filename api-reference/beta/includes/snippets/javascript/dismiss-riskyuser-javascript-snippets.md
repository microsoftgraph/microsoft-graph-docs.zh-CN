---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 525f3819a68e79648494f692bb5d79e6cbef2dcd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const dismiss = {
  userIds: [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
};

let res = await client.api('/riskyUsers/dismiss')
    .version('beta')
    .post(dismiss);

```