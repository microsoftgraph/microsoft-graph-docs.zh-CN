---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 498934c64a95165af4a77a08029fe57461586fd32d3850491d1768459530515e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277263"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let namedLocations = await client.api('/identity/conditionalAccess/namedLocations')
    .filter('microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq \'CA\')')
    .get();

```