---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32ae5b2459908693112986bc8daa10ae67ce91ef
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60690110"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appManagementPolicy = {
 '@odata.id':'https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}'
};

await client.api('/servicePrincipals/{id}/appManagementPolicies/$ref')
    .version('beta')
    .post(appManagementPolicy);

```