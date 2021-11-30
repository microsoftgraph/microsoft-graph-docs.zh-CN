---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5390af1fdb60c2548c7772bfb16a9f120b9b32c
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224595"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let customSecurityAttributeDefinitions = await client.api('/directory/customSecurityAttributeDefinitions')
    .version('beta')
    .filter('name eq \'Project\' and status eq \'Available\'')
    .get();

```