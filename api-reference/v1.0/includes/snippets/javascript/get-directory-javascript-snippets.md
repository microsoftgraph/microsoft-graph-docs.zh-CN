---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8fb8e9f5008aa54b23a567b9b294b7cbea2c42f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618022"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/deletedItems/{object-id}')
    .get();

```