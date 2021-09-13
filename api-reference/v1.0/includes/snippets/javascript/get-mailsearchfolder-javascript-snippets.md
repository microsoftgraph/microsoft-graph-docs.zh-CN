---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8308a3468f7c201c9ea7679e430cab4378c0c53c0ddea503623f655d8a7dba48
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332571"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mailFolder = await client.api('/me/mailFolders/AAMkAGVmMDEzN')
    .get();

```