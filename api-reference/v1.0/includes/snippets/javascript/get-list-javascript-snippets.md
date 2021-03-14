---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56fc7e8f000ee3a07955ae52971a0a724ba6b6eb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791143"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let list = await client.api('/sites/{site-id}/lists/{list-title}')
    .get();

```