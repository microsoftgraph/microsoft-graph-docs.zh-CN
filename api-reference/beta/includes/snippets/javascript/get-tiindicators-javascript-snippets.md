---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7312921fb54a9fe579bb6e29c758323e27bc3a96
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521221"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/tiIndicators')
    .version('beta')
    .get();

```