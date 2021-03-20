---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0eed38013196ed3179f93464f9862d08bea932cb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947445"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let namedLocations = await client.api('/identity/conditionalAccess/namedLocations')
    .version('beta')
    .filter('microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq \'CA\')')
    .get();

```