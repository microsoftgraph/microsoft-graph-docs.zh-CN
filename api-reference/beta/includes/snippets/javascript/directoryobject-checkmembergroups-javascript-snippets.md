---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0008a8c18105e363954deec2388848bdbe52fc8e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793797"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  groupIds: [
        'fee2c45b-915a-4a64-b130-f4eb9e75525e',
        '4fe90ae7-065a-478b-9400-e0a0e1cbd540'
  ]
};

await client.api('/me/checkMemberGroups')
    .version('beta')
    .post(string);

```