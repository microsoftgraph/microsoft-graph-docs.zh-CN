---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f3df6fd6e888abc4e8d9532d72e8dd928235a34
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60995206"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let softwareOathMethods = await client.api('/me/authentication/softwareOathMethods')
    .version('beta')
    .get();

```