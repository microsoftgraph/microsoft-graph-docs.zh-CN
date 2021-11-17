---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8fdcdc90f7fee015bac09a7468062a31bac5cb40eb0c5f4f8d94c41eb76e7b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332900"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/messages/{id}/send')
    .version('beta')
    .post();

```