---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46dc590bbbb31387f99245d6cee81f383f6ff9f3c0038a8223d8d0b6d0ca5c01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221251"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/contactFolders/{id}')
    .version('beta')
    .delete();

```