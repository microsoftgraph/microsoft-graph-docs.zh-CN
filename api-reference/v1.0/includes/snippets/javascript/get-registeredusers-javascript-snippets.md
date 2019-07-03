---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8c1ce6bb2e178aa5fb30b4b6d3e193819d3917cf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509561"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}/registeredUsers')
    .get();

```