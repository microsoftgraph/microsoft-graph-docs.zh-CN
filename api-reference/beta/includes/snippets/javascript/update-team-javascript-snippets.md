---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 192501c90adee4eaed9908b4d35417123ef39bece30e9bbd2a2f70334f854138
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279564"
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
    giphyContentRating: 'strict'
  },
  discoverySettings: {
    showInTeamsSearchAndSuggestions: true
  }
};

await client.api('/teams/{id}')
    .version('beta')
    .update(team);

```