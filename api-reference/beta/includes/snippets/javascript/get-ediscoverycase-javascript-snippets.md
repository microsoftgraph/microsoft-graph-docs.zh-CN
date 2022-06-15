---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2382b9479c24b2a3d7874bd4fd1804a2c6617f9
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096166"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ediscoveryCase = await client.api('/security/cases/eDiscoverycases/22aa2acd-7554-4330-9ba9-ce20014aaae4')
    .version('beta')
    .get();

```