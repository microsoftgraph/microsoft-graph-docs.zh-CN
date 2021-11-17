---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b59861429a197cbb022079341fc3de37de3a9ccac3d94af1be6ed8c27c75ebe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158670"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}')
    .version('beta')
    .delete();

```