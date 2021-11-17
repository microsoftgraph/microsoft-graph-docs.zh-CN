---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5d8b12cb8a976510a0c8b5ec4970cad1cd34880
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "61031756"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/kim@contoso.com/authentication/softwareOathMethods/b172893e-893e-b172-3e89-72b13e8972b1')
    .version('beta')
    .delete();

```