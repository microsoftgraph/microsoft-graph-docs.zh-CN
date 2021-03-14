---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46ffe54489c8e9794058dd762dbca94e683c28fb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790337"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let presence = await client.api('/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647')
    .get();

```