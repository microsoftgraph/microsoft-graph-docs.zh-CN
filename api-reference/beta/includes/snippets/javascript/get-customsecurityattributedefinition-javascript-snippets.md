---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8861489f630d6d269698599beb10d2be141dcbe2
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225776"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let customSecurityAttributeDefinition = await client.api('/directory/customSecurityAttributeDefinitions/Engineering_ProjectDate')
    .version('beta')
    .get();

```