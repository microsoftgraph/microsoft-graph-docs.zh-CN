---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d979d51e271349463ae1dadd50da799153cdc882
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226241"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipal = await client.api('/servicePrincipals/{id}')
    .version('beta')
    .select('customSecurityAttributes')
    .get();

```