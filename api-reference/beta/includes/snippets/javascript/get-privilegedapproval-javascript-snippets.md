---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e20e18cf8826e7a52d532c5d689eb23a50671e66
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792223"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedApproval = await client.api('/privilegedApproval')
    .version('beta')
    .get();

```