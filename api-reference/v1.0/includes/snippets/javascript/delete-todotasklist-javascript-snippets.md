---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d1eec4403e0ee633d1519a429fbb0f6920a903051c28af3ef4544f374540e60
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162152"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/todo/lists/AAMkADIyAAAhrbPXAAA=')
    .delete();

```