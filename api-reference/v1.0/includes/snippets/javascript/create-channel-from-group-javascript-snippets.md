---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5b75c9b4eb67b789f89dd208bb201a0864f1206
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373450"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
  displayName: "Architecture Discussion",
  description: "This channel is where we debate all future architecture plans",
  membershipType: "standard"
};

let res = await client.api('/teams/{id}/channels')
    .post(channel);

```