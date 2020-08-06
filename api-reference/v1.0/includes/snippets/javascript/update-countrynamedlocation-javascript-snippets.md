---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 095cf616dce1949a63521288b3788561d1af158f
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567092"
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

let res = await client.api('/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959')
    .update(namedLocation);

```