---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed2b46590bedc6b095e9bf39cab08315149fc7bfaa97801a4df4e296c0928bb8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332390"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let credentialUserRegistrationsSummaries = await client.api('/tenantRelationships/managedTenants/credentialUserRegistrationsSummaries')
    .version('beta')
    .get();

```