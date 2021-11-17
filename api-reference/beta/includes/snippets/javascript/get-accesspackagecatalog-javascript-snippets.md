---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f1cda7edd24ca56318a6d1c37d70148d7e1007a49d872f3a42fb2195584231a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902778"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageCatalog = await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}')
    .version('beta')
    .get();

```