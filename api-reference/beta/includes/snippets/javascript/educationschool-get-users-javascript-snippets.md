---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc11a050f003fc7607b7b802b2bdb50ef1f57b617997359b000810a01f03d188
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219054"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/education/schools/10002/users')
    .version('beta')
    .get();

```