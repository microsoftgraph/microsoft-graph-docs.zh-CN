---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e69086b30046c8679a84746f700db10d582d1f53b8e176ff0e11d253865cfd21
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277743"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/todo/lists/AAMkADIyAAAhrbPXAAA=')
    .version('beta')
    .delete();

```