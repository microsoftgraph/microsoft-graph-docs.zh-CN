---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52cb617f79ee3cd4ffa727f5ff5feedb24cd0739
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806980"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let namedLocation = await client.api('/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959')
    .version('beta')
    .get();

```