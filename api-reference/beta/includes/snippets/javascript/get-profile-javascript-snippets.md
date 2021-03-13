---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2da69a74e708c1a05d37993544bfb5213a0ade22
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801992"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let profile = await client.api('/me/profile')
    .version('beta')
    .expand('skills($select=displayName)')
    .get();

```