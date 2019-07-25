---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2f8830c001b746892f38d63bea30b3a46ba9e857
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35704920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/inbox/messageRules')
    .get();

```