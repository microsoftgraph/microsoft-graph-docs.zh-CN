---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e2041bd9f0bb76e8d4df20f7156c0e75d7b6d775
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458033"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forceDelete = {
  disableUserAccounts: true
};

let res = await client.api('/domains/{id}/forceDelete')
    .version('beta')
    .post(forceDelete);

```