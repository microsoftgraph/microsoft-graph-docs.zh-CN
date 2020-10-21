---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 777ea8bafe5ac5673f9f6eb3a0d3c5060bb3d36e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617019"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/{id}/messages/delta')
    .header('Prefer','odata.maxpagesize=2')
    .get();

```