---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2d875a498f6d0894211ac89601144e7c9004c7450bf22f7b36ac7433a264792
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220873"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sections = await client.api('/me/onenote/sections')
    .version('beta')
    .get();

```