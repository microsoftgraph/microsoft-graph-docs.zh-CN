---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db37ca72cabb05724d7b2f891b9c8bd8669e3010
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781873"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/drive/items/{bundle-id}?expand=children')
    .version('beta')
    .get();

```