---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 956d8a179baca94ee5c9f574ae6d3cad924d2f01
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096242"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ediscoveryCase = {
    displayName: 'My Case 1 - Renamed',
    description: 'Updated description'
};

await client.api('/security/cases/eDiscoverycases/22aa2acd-7554-4330-9ba9-ce20014aaae4')
    .version('beta')
    .update(ediscoveryCase);

```