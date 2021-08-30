---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ac587c9f6d81e3f86da8026a6fc88dba15502c5631bf5d2162bf9ac3bd2374c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104711"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appRoleAssignments = await client.api('/servicePrincipals/8e881353-1735-45af-af21-ee1344582a4d/appRoleAssignments')
    .version('beta')
    .get();

```