---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6c540d20ce5aa650a90904fb7a89755f2804550
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959068"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignments = await client.api('/roleManagement/directory/roleAssignments')
    .version('beta')
    .filter('roleDefinitionId eq \'62e90394-69f5-4237-9190-012177145e10\'')
    .expand('principal')
    .get();

```