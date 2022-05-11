---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56de769946402d5abda82e0b3b24913a21ceee12
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315379"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let samlOrWsFedExternalDomainFederation = await client.api('/directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation')
    .version('beta')
    .filter('domains/any(x: x/id eq \'contoso.com\')')
    .get();

```