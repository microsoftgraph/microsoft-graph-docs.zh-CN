---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 147bd12ee345cf1baf7a25be7a9d7cb7e9c73d5d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796414"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/directory/deletedItems/{object-id}')
    .get();

```