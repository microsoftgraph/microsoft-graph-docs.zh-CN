---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ced46f440c47aac091f0de2db116a155cf7f8f10
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800741"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
  displayName: 'Architecture Discussion',
  description: 'This channel is where we debate all future architecture plans',
  membershipType: 'standard'
};

await client.api('/teams/{id}/channels')
    .post(channel);

```