---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b16bc6567cee2bcdc7fd13a09dc727134e1c0c07
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807599"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let internalSponsors = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}/internalSponsors')
    .version('beta')
    .get();

```