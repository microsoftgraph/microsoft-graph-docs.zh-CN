---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5978324387fbed313862967a871596caa2799636
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147664"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const associateWithHubSites = {
   hubSiteUrls: [
      'https://graph.microsoft.com/v1.0/sites/{site-id}'
   ],
   propagateToExistingLists: false
};

await client.api('/sites/{site-id}/contentTypes/{contentTypeId}/associateWithHubSites')
    .post(associateWithHubSites);

```