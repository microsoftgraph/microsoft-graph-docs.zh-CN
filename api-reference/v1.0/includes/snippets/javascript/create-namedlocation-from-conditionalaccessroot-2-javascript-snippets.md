---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5cc3cf3ec8844b5c9a2ba82cc8e9cfa693e52b9cdc6fb653d18261fb75c26e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279197"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const namedLocation = {
    '@odata.type': '#microsoft.graph.countryNamedLocation',
    displayName: 'Named location with unknown countries and regions',
    countriesAndRegions: [
        'US',
        'GB'
    ],
    includeUnknownCountriesAndRegions: true
};

await client.api('/identity/conditionalAccess/namedLocations')
    .post(namedLocation);

```