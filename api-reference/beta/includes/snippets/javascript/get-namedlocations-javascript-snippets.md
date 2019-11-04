---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 003a3dc84b4e5579d1b4b9ff98f3faad3eec4b18
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936680"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/conditionalAccess/namedLocations')
    .version('beta')
    .filter('microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')')
    .get();

```