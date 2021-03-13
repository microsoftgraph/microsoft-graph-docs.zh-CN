---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5714cf28cd555aae62fe8340cea663e1c53f4f85
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809259"
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

await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels')
    .version('beta')
    .post(channel);

```