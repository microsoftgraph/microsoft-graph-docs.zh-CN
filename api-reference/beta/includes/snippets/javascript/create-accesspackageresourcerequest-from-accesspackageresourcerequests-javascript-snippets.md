---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff483b33f0645593f1e48924e37bdd506c1fcc2e
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911804"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageResourceRequest = {
  catalogId:"26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  requestType: "AdminAdd",
  justification: "",
  accessPackageResource: {
     displayName: "Sales",
     description: "https://contoso.sharepoint.com/sites/Sales",
     url: "https://contoso.sharepoint.com/sites/Sales",
     resourceType: "SharePoint Online Site",
     originId: "https://contoso.sharepoint.com/sites/Sales",
     originSystem: "SharePointOnline"
  }
};

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageResourceRequests')
    .version('beta')
    .post(accessPackageResourceRequest);

```