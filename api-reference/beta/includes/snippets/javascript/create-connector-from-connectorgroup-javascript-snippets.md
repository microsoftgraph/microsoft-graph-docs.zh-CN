---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c90d667a05f9334d39f14f199b72c86d874674198895380ba3f39744994f0d9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902430"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connector = {
  '@odata.id': 'https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}'
};

await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref')
    .version('beta')
    .post(connector);

```