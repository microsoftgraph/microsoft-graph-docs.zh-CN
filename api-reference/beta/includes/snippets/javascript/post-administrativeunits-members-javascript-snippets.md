---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc833fc4e6068d43505bd0266778b51744875631
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890216"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.type': '#Microsoft.Graph.Group',
  description: 'Self help community for golf',
  displayName: 'Golf Assist',
  groupTypes: [
    'Unified'
  ],
  mailEnabled: true,
  mailNickname: 'golfassist',
  securityEnabled: false
};

await client.api('/administrativeUnits/{id}/members')
    .version('beta')
    .post(directoryObject);

```