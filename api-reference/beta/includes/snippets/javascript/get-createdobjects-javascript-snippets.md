---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 53d23056d9832a9ef5935564785e75741a7f341b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520225"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/createdObjects')
    .version('beta')
    .get();

```