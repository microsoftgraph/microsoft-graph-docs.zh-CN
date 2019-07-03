---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9475b9b309ec5019a30f37b4f627a92b5d464b96
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510213"
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
    .update({group : group});

```