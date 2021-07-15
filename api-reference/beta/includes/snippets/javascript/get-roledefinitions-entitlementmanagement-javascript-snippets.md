---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec9bc8fe0f19f332b5996049dca55c186dee764e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442272"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleDefinitions = await client.api('/roleManagement/entitlementManagement/roleDefinitions')
    .version('beta')
    .get();

```