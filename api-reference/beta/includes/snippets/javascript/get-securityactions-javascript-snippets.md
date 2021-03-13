---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 030b9d6bef49dba29d03c9f10d5af17dae0fb47c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799720"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let securityActions = await client.api('/security/securityActions')
    .version('beta')
    .get();

```