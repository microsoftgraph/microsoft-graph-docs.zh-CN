---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbcb213e26b726742500a0021959e725be1d85d21b7c9b5dd7d76f363d2956d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904212"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  memberSettings: {
    allowCreateUpdateChannels: true
  },
  messagingSettings: {
    allowUserEditMessages: true,
    allowUserDeleteMessages: true
  },
  funSettings: {
    allowGiphy: true,
    giphyContentRating: 'strict'
  },
  discoverySettings: {
    showInTeamsSearchAndSuggestions: true
  }
};

await client.api('/groups/{id}/team')
    .version('beta')
    .put(team);

```