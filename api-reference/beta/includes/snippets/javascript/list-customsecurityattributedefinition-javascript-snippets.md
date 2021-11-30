---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c57d2251867dc56afa2aeb4a35dce44fdd03562
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224630"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let customSecurityAttributeDefinitions = await client.api('/directory/customSecurityAttributeDefinitions')
    .version('beta')
    .get();

```