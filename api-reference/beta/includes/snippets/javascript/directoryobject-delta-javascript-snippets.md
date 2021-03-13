---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3c0a252314ab3b850c9e1823c4dfcc7a862e44e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789290"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/directoryObjects/delta')
    .version('beta')
    .filter('isOf(\'Microsoft.Graph.User\') or isOf(\'Microsoft.Graph.Group\')')
    .get();

```