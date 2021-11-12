---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93bff3dec55af41f485fa76af96c4722964dea41113d0418a4299bb82270f935
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162926"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectorGroup = {
  '@odata.id': 'https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}'
};

await client.api('/onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf/$ref')
    .version('beta')
    .post(connectorGroup);

```