---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc241334ecc1f88c2b4ed7cdc31240da8b270bdd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806935"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let versions = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}/versions')
    .get();

```