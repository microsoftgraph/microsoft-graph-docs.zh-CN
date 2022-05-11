---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c4909bdd921c10e014203cdb4f99f31727d5c7a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let domains = await client.api('/directory/federationConfigurations/microsoft.graph.samlOrWsFedExternalDomainFederation/f1e11a04-0244-4592-99df-b01cfaadce15/domains')
    .version('beta')
    .get();

```