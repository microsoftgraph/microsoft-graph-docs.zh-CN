---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68d641b1d6ab6a810867baa411b244355de3a4f4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792841"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let owners = await client.api('/applications/{id}/owners')
    .version('beta')
    .get();

```