---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a751a2dfd7b7306ceaf649c4b26598c7d895f01
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46813705"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
 isMembershipLimitedToOwners: true,
  memberSettings: {
    allowCreateUpdateChannels: true
  },
  messagingSettings: {
    allowUserEditMessages: true,
    allowUserDeleteMessages: true
  },
  funSettings: {
    allowGiphy: true,
    giphyContentRating: "strict"
  },
  discoverySettings: {
    showInTeamsSearchAndSuggestions: true
  }
};

let res = await client.api('/teams/{id}')
    .version('beta')
    .update(team);

```