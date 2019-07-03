---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c1c50c164319b4b9a1e39f7dfeef2696fff2555d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477988"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailboxSettings')
    .version('beta')
    .get();

```