---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8f097a99d2e8b17efd5de50ed4cacc18ac42f9ab
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467694"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd')
    .select('allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount')
    .get();

```