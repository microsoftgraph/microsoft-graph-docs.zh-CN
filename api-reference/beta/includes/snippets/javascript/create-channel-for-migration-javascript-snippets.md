---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7864812e565d0fcc1df5eb448e432aeed9863fd4
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753789"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
  @microsoft.graph.channelCreationMode: "migration",
  displayName: "Architecture Discussion",
  description: "This channel is where we debate all future architecture plans",
  membershipType: "standard",
  createdDateTime: "2020-03-14T11:22:17.067Z"
};

let res = await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels')
    .version('beta')
    .post(channel);

```