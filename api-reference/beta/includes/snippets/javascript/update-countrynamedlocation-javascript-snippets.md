---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98cd6821f2fc0b43cbc00c94260a090521479c46
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2020
ms.locfileid: "43061987"
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
    .version('beta')
    .update(namedLocation);

```