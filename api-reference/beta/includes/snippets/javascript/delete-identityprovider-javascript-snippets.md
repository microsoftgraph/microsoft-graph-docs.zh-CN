---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d347badf1fb43a705edb8c925aeffc928389030f
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566805"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProviders/{id}')
    .version('beta')
    .delete();

```