---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a70506e89b600190f625644e876aa3dc9ec24ed8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615214"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/taskFolders')
    .version('beta')
    .get();

```