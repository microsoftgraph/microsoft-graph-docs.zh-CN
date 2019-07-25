---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fe6b28e778100cfbfb6c5d114cea02e9dfe141e9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724529"
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
    giphyContentRating: "strict"
  },
  discoverySettings: {
    showInTeamsSearchAndSuggestions: true
  }
};

let res = await client.api('/teams/{id}')
    .version('beta')
    .update({team : team});

```