---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a342b550db2788367eee4a57682f6889c1e31d68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60729449"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contentType = {
  contentType: 'https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101'
};

await client.api('/sites/{site-id}/lists/{list-id}/contentTypes/addCopy')
    .version('beta')
    .post(contentType);

```