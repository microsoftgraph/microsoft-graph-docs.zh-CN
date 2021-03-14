---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5201f2489d7bc8bd37220e30d1b3968cd09d4673
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803780"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const namedLocation = {
    '@odata.type': '#microsoft.graph.countryNamedLocation',
    displayName: 'Updated named location without unknown countries and regions',
    countriesAndRegions: [
        'CA',
        'IN'
    ],
    includeUnknownCountriesAndRegions: false
};

await client.api('/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959')
    .update(namedLocation);

```