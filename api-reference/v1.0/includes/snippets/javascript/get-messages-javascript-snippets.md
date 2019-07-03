---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d6f0a5730e14a2620afdbc6f51630a89119da8d7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509388"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages')
    .select('sender,subject')
    .get();

```