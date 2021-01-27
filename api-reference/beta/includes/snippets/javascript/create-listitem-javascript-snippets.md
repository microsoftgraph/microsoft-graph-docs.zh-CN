---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b26a684830655bfae59c51260d43ce04ef7f2cf
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015483"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const listItem = {
  fields: {
    Title: "Widget",
    Color: "Purple",
    Weight: 32
  }
};

let res = await client.api('/sites/{site-id}/lists/{list-id}/items')
    .version('beta')
    .post(listItem);

```