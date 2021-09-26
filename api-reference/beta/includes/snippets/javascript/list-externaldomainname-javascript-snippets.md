---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c4909bdd921c10e014203cdb4f99f31727d5c7a
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766521"
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