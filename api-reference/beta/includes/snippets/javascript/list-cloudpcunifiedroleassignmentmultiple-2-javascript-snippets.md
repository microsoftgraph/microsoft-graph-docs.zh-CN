---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1527a5e9118a6dd3a2ff619ac1223eeec9f9729a4244e27d92063b55405de133
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278915"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignments = await client.api('/roleManagement/cloudPC/roleAssignments')
    .version('beta')
    .filter('roleDefinitionId eq \'b5c08161-a7af-481c-ace2-a20a69a48fb1\'')
    .get();

```