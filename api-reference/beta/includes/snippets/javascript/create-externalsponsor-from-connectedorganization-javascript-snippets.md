---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66ff9b4f494f99834d3c5f280dea11285a8222c0
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810182"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/beta/users/{id}"
};

let res = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors/$ref')
    .version('beta')
    .post(directoryObject);

```