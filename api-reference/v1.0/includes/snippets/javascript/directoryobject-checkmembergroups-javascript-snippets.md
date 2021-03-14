---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b96ee5849d2395eb87f88e9781b0566e226609eb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  groupIds: [
        'fee2c45b-915a-4a64b130f4eb9e75525e',
        '4fe90ae065a-478b9400e0a0e1cbd540'
  ]
};

await client.api('/directoryObjects/{id}/checkMemberGroups')
    .post(string);

```