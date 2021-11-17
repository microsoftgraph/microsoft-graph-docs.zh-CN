---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 540b37af32d94540b8c36b4caf6860e3a26c7edd5bf4f7f58c1e6e077d688770
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278772"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let list = await client.api('/sites/{site-id}/lists/{list-id}')
    .version('beta')
    .get();

```