---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14f229af2594a7092fa569871ba9cf1086b91adb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621241"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/special/{name}/children')
    .version('beta')
    .get();

```