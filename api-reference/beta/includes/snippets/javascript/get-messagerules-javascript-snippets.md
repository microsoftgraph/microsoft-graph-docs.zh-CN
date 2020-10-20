---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 099074925568b22da84040005f5fc67336d2c15a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612493"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/inbox/messagerules')
    .version('beta')
    .get();

```