---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 629c7c8864a4c31ec745108857fc5727b7cd65bd
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224511"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const allowedValue = {
    id: 'Alpine',
    isActive: 'true'
};

await client.api('/directory/customSecurityAttributeDefinitions/Engineering_Project/allowedValues')
    .version('beta')
    .post(allowedValue);

```