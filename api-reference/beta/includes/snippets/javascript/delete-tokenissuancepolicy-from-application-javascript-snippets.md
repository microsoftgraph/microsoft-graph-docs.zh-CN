---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5da5700b8e6c72fc426107aad619cfddf344e8e5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785347"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/tokenIssuancePolicies/{id}/$ref')
    .version('beta')
    .delete();

```