---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51c24e0213f754f79d6a146ca4f789c3bd404e85
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095980"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/security/cases/eDiscoverycases/22aa2acd-7554-4330-9ba9-ce20014aaae4')
    .version('beta')
    .delete();

```