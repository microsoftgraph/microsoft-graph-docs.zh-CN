---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36394eaceaf2f6a6a4b895c0f1424a1b44a8ff3c
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806218"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/oauth2permissiongrants/delta')
    .version('beta')
    .get();

```