---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40c2801721fe7dd400442f7bbd7ed9fbf83f1895e553cb8558e0b90b2fe0f554
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219977"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMemberOf = await client.api('/devices/{id}/transitiveMemberOf')
    .version('beta')
    .get();

```