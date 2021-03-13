---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e869ed6d37eb8438687c8d6438a8a436b58a0fe0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803773"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const place = {
  '@odata.type': 'microsoft.graph.room',
  nickname: 'Conf Room',
  building: '1',
  label: '100',
  capacity: 50,
  isWheelChairAccessible: false
};

await client.api('/places/cf100@contoso.com')
    .version('beta')
    .update(place);

```