---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 050feaba37e614ceb5e8be464a3631c8d53b9736
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428861"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  groupIds: [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
};

let res = await client.api('/directoryObjects/{id}/checkMemberGroups')
    .post(string);

```