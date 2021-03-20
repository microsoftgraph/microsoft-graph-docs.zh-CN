---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3c0a252314ab3b850c9e1823c4dfcc7a862e44e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946644"
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