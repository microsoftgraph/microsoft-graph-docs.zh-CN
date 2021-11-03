---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7964dd5e539b2ee5311cb6b9e21a3e496bf50084
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60729407"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const associateWithHubSites = {
   hubSiteUrls: [
      'https://graph.microsoft.com/beta/sites/id'
   ],
   propagateToExistingLists: false
};

await client.api('/sites/{siteId}/contentTypes/{contentTypeId}/associateWithHubSites')
    .version('beta')
    .post(associateWithHubSites);

```