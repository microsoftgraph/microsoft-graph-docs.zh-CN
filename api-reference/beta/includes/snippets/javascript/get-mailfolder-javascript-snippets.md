---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3dd0b805560fa899fcdd81e4dc8c4d28ccc311e39bf28ac82628a936e3618ea2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333119"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mailFolder = await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .version('beta')
    .get();

```