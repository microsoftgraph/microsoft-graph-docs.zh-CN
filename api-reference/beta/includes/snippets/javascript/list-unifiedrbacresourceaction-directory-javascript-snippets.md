---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85da1ed81ca56428c9911b92e27dbf45f05cef27
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let resourceActions = await client.api('/roleManagement/directory/resourceNamespaces/microsoft.directory/resourceActions')
    .version('beta')
    .get();

```