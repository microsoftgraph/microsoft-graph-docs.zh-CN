---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b851f05028154005db1e99016e0c363b06385c1
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66446584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/domains/contoso.com/promote')
    .version('beta')
    .post();

```