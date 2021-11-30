---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9b456f507024ab22926db727b3badab5afd67d9
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225959"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let allowedValues = await client.api('/directory/customSecurityAttributeDefinitions/Engineering_Project/allowedValues')
    .version('beta')
    .get();

```