---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62129b52dee7d58c61783da13592ec557d8b8cde403aeb14d55739d4140f5b09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218505"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{item-id}/unfollow')
    .version('beta')
    .delete();

```