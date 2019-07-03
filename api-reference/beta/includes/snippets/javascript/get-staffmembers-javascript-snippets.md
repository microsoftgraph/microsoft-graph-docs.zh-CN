---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9a1ac139bf7cb1f07ce91a790e5f181fc06abf0d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521133"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers')
    .version('beta')
    .get();

```