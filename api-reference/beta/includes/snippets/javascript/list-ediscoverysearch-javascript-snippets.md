---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24d27b39c08284fe31048c8bc0f1b093c261974e
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092892"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let searches = await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches')
    .version('beta')
    .get();

```