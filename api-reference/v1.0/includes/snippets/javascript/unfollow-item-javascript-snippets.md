---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae1a4523d0cdc10204e13b88624c03b2f171ba96
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804913"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{item-id}/unfollow')
    .post();

```