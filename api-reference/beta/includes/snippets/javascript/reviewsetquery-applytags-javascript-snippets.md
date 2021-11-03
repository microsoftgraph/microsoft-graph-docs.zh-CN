---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74c64a8f0a95a4a628b9a70cb5a5382622f289575897b06b3e76f9cd927646b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105794"
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