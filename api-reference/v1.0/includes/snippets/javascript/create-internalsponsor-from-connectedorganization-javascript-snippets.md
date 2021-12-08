---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ad69f7aadb90dcdd63dae92731bb90bb4030648
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336348"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/users/{id}'
};

await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}/internalSponsors/$ref')
    .post(directoryObject);

```