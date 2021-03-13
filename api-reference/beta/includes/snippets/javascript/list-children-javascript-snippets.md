---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e617cc3a85aba92fd70a3338b6f6bb4349e799a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808998"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/drives/{drive-id}/items/{item-id}/children')
    .version('beta')
    .get();

```