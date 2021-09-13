---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62db9f505480522708eb98f2cd085d0ac11eabfe
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignments = await client.api('/roleManagement/directory/roleAssignments')
    .filter('roleDefinitionId eq \'62e90394-69f5-4237-9190-012177145e10\'')
    .expand('principal')
    .get();

```