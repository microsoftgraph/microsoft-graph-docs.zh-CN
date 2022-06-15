---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6573dbfff14ec35cb3d6c17645dc0671db737954
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093804"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let reviewSets = await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/reviewSets')
    .version('beta')
    .get();

```