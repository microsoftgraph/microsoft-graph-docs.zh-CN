---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78dd60340f8289f2098e519bb8047b68ed7eee72
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793358"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07')
    .version('beta')
    .delete();

```