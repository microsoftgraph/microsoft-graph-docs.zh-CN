---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abb4d7ff11e3b8a5a5eb74facc080293ebfc1cbd
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224627"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let customSecurityAttributeDefinitions = await client.api('/directory/customSecurityAttributeDefinitions')
    .version('beta')
    .filter('attributeSet eq \'Engineering\' and status eq \'Available\' and type eq \'String\'')
    .get();

```