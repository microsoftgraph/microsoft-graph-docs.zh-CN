---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e719c6a9c62f53b40cc3c265f9ba6dbc4c542eb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315770"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let samlOrWsFedExternalDomainFederation = await client.api('/directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation')
    .get();

```