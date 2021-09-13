---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fb3f93f2c881185e7482395da09f9e4a9994d57fa42e6efd25436ab52afc1bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/mailFolders/{id}')
    .delete();

```