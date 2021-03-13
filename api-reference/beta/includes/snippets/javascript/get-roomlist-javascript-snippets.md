---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97aa43a528b573c72cfa70a60fef40a042a2ee4e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804687"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let place = await client.api('/places/bldg1@contoso.com')
    .version('beta')
    .get();

```