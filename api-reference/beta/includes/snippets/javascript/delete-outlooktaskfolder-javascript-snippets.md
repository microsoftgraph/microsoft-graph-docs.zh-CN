---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a157ea75ff74e7ebcfcbc66f57b3e8562e6d209b00e8db927d1f2a74e9a65dc9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903505"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/outlook/taskFolders/AAMkADIyAAAhrbPXAAA=')
    .version('beta')
    .delete();

```