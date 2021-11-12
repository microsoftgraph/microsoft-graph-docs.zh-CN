---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ae1481d6c122cca5ba9cf323f30e47f0be826a630a0a8503d99213c95056080
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162694"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mailFolders = await client.api('/me/mailFolders/?includeHiddenFolders=true')
    .version('beta')
    .get();

```