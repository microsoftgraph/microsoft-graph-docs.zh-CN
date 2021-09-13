---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e70cdb2696c7c535bbd0e8853f6835cc68450512dc607418cf968999009ceeb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332569"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mailFolder = await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .get();

```