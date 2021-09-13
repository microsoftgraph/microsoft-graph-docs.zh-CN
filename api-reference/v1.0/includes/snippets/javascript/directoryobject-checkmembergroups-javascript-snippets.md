---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0fa222cf1dc039aef5fc7491e3f25f3ae778e57c7edb9b52642787416dfdd37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903358"
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