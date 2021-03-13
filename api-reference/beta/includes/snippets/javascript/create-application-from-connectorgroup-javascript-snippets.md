---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23de1c094b0e001d158afd2f42ce058c8f4023f4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802595"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectorGroup = {
  '@odata.id': 'https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}'
};

await client.api('/applications/{id}/connectorGroup/$ref')
    .version('beta')
    .put(connectorGroup);

```