---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 95aa02f03dba39d669e1f75c245f3edff4b6b8f1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493194"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  groupIds: [
    "groupIds-value"
  ]
};

let res = await client.api('/me/checkMemberGroups')
    .post(String);

```