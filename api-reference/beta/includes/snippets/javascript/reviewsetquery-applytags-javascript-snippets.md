---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df97ffc816b079858c5a58bc0b16168f62839226
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772827"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const applyTags = {
    tagsToAdd: [
        {
            id: 'b4798d14-748d-468e-a1ec-96a2b1d49677'
        }
    ]
};

await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/reviewsets/6c95c2a6-31fa-45a8-93ef-dd4531974783/queries/b4798d14-748d-468e-a1ec-96a2b1d49677/applyTags')
    .version('beta')
    .post(applyTags);

```