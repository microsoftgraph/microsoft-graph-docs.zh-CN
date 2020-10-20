---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cee953866b593dcd90024bdaf206fd851a90792b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604170"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/items/{item-id}/content?format=%7Bformat%7D')
    .version('beta')
    .get();

```