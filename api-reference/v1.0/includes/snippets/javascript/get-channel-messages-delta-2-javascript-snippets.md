---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae9278e4a1132a27daa3196ba38b8dff0b018a9e
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905019"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels/{id}/messages/delta')
    .skiptoken('c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA=')
    .get();

```