---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b107b3483d835f464c15c235bc24f652cd55018222a4260edf0138e89f5985d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278751"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let programControlTypes = await client.api('/programControlTypes')
    .version('beta')
    .get();

```