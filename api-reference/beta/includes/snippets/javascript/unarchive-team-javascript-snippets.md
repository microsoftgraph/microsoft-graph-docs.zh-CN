---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: addd0b3414ba665869795f47037f0ca19ad0670b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335219"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/unarchive')
    .version('beta')
    .post();

```