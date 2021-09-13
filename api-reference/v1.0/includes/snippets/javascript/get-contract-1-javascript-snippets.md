---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c2abbdff9ef70e8d51f21d48276d8c8038d85ce8534fac0c6fca7ded09a8ebf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333991"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contract = await client.api('/contracts/{id}')
    .get();

```