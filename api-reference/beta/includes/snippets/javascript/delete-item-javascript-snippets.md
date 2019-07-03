---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3fe0b759fdc8ea025d49ffad7c8e1ab2f990ae06
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}')
    .version('beta')
    .delete();

```