---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 701b91887d88a32d1ef6dea369a4a90aee680c4c
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869013"
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