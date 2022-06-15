---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9806fda0402e9f327b3a5aa7c1a16f129c50a10a
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092947"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ediscoveryHoldPolicy = await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/legalholds/783c3ea4-d474-4051-9c13-08707ce8c8b6')
    .version('beta')
    .get();

```