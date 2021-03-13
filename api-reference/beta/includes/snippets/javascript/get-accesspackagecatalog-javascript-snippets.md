---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58b89ccd4a3c8e5b73b34a48560cb6bf8baa2abe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792254"
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