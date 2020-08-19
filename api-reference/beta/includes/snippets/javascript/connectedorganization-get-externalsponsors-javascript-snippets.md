---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f740e76a258e84f3dc62a77fa098db4abad90f26
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810220"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors')
    .version('beta')
    .get();

```