---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abf48f4fef127d24586ae45b3bf769d4c3ab259a1594d1d38dbdc33481187207
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106021"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columns = await client.api('/sites/{site-id}/lists/{list-id}/columns')
    .version('beta')
    .get();

```