---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db6b92ff1baf16be8989c526fb75b4652dd67cfc
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621167"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/versions')
    .version('beta')
    .get();

```