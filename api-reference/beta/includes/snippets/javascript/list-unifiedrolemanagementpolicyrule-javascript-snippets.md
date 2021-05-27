---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 574bd8c6b80217bc1b71da3b115c1339be6d7dbb
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668563"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rules = await client.api('/policies/roleManagementPolicies/ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba/rules')
    .version('beta')
    .get();

```