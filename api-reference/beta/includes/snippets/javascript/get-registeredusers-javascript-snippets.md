---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b4bb85e0eed7e0d62609ac8ba5b64e6887011a48
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520455"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}/registeredUsers')
    .version('beta')
    .get();

```