---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 402f1b4941b8dbf34aaa8bb7f319dce41eacaebbce3742987b1792f7e029f992
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902473"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleDefinition = await client.api('/roleManagement/entitlementManagement/roleDefinitions/ba92d953-d8e0-4e39-a797-0cbedb0a89e8')
    .version('beta')
    .get();

```