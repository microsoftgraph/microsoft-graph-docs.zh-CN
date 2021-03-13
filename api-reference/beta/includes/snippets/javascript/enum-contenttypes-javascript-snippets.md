---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de6493edcdd5493cedca3b1ecd396b7a743bd9c8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contentTypes = await client.api('/sites/{site-id}/contentTypes')
    .version('beta')
    .get();

```