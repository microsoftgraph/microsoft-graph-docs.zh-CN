---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fcd5e1c5281572e8a5d5efe4cd86070b222162f5
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636490"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: "description-value",
  displayName: "displayName-value",
  groupTypes: [
    "groupTypes-value"
  ],
  mail: "mail-value",
  mailEnabled: true,
  mailNickname: "mailNickname-value"
};

let res = await client.api('/groups/{id}')
    .version('beta')
    .update(group);

```