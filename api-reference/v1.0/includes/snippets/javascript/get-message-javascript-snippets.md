---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c390a266face6be44389f0158a8d06fdfdf9c95a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493604"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADhMGAAA=')
    .get();

```