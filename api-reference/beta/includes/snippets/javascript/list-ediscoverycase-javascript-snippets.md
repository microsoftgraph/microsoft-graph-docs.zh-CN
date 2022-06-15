---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aaeade38d1d0d94949e17bba4266e73fded7b709
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ediscoveryCases = await client.api('/security/cases/ediscoveryCases')
    .version('beta')
    .get();

```