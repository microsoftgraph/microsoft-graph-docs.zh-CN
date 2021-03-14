---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72484ff678699675f497639b17ca572839a917c1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805569"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2')
    .delete();

```