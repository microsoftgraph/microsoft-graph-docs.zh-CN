---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8122fabea5ca26efa3acf9d166ac279f7c76fce
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565985"
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

let res = await client.api('/identity/conditionalAccess/namedLocations')
    .post(namedLocation);

```