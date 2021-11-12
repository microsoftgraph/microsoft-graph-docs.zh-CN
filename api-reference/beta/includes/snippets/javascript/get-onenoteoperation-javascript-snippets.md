---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ee873751d528846f8cc8c3a4de5d9833e93b729eb396ad44b1ac979c24ce555
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219744"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onenoteOperation = await client.api('/me/onenote/operations/{id}')
    .version('beta')
    .get();

```