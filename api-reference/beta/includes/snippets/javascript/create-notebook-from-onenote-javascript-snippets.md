---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60a16b2007f4aff095b2d7fb26ab6895ef65ecfbae0bfa6a26af1950197ffeaf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218487"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const notebook = {
    displayName: 'My Private notebook'
};

await client.api('/me/onenote/notebooks')
    .version('beta')
    .post(notebook);

```