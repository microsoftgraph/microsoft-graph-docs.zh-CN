---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 268d059ea5088b0491bd7b0d48f9870e07b2294228bdd483c403b5c6b1ba0da6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162324"
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
  }
};

await client.api('/teams/{id}')
    .update(team);

```