---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ea46f4f00424b586c4d79facca28a6565fe8806b21dbc8059d4140351ecc24d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103818"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleDefinition = await client.api('/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c')
    .version('beta')
    .expand('inheritsPermissionsFrom')
    .get();

```