---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4125721f7d3fa6004c4954259d737b5babecef56
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478249"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd')
    .version('beta')
    .select('allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount')
    .get();

```