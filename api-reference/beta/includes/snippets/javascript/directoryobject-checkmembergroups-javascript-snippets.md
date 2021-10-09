---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64d3d7e5403443284c33b698380fdf45127585801618286ada14f1fe5fbd2ebb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161282"
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