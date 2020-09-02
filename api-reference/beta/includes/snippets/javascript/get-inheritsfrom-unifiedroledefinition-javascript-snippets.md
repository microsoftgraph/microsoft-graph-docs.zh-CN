---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7a6959f3d2689e0d51ae2b7a66dec50ab1d128d
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330329"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c')
    .version('beta')
    .expand('inheritsPermissionsFrom')
    .get();

```