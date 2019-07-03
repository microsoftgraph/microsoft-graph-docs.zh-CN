---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d27926a091e7f2319c24290d9922649ed8b5bf6d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478647"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')')
    .version('beta')
    .get();

```