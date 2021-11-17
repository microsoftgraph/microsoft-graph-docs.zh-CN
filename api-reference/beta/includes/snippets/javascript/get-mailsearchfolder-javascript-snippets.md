---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f7fb31ce32a6348cc5dbcf01d759a50a6da30ca31e363b27c59c0b1e5e66f15
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333117"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mailFolder = await client.api('/me/mailFolders/AAMkAGVmMDEzN')
    .version('beta')
    .get();

```