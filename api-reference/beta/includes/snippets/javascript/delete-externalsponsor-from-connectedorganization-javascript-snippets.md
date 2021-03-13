---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 783a82fb194a87c5c1b92b550f45ecfff8467cb8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809759"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref')
    .version('beta')
    .delete();

```