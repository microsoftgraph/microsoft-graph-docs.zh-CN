---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f82edb9814575825e3fb4671ba039ad80867d82
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802366"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let apiConnectors = await client.api('/identity/apiConnectors')
    .version('beta')
    .get();

```