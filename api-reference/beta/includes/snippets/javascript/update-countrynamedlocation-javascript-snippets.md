---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f13668444d5b87fec2bd269576a08244524be96f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937107"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const namedLocation = {
    @odata.type: "#microsoft.graph.countryNamedLocation",
    displayName: "Updated named location without unknown countries and regions",
    countriesAndRegions: [
        "CA",
        "IN"
    ],
    includeUnknownCountriesAndRegions: false
};

let res = await client.api('/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959')
    .version('beta')
    .update(namedLocation);

```