---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a2d1cd16ccd8a492497c4cc109d68773b52578e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465366"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/schemaExtensions')
    .version('beta')
    .filter('id eq \'graphlearn_test\'')
    .get();

```