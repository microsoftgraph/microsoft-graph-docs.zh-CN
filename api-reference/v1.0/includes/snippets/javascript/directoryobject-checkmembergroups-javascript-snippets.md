---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8e81b5afbfb798f6d233c0822ada05c8147975af
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493338"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  groupIds: [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
};

let res = await client.api('/directoryObjects/{id}/checkMemberGroups')
    .post(String);

```