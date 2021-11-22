---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe783fd5d241b27dc27343bba39435204ecbfa4858d7b7b4c34f10c4447b1669
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219025"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let childFolders = await client.api('/me/mailFolders/AAMkAGVmMDEzM/childFolders?includeHiddenFolders=true')
    .version('beta')
    .get();

```