---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 906953f20b09fb6029abf765a5774c320c4e7d4a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810157"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}/internalSponsors')
    .version('beta')
    .get();

```