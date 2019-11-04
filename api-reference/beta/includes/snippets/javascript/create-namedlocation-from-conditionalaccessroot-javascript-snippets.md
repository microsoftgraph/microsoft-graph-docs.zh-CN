---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95ee551fa17dd22a739d6688408c0e91d002277d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936629"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const namedLocation = {
    @odata.type: "#microsoft.graph.countryNamedLocation",
    displayName: "Named location with unknown countries and regions",
    countriesAndRegions: [
        "US",
        "GB"
    ],
    includeUnknownCountriesAndRegions: true
};

let res = await client.api('/conditionalAccess/namedLocations')
    .version('beta')
    .post(namedLocation);

```