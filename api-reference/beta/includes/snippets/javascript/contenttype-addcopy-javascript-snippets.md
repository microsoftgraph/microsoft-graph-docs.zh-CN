---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 625fe0021c8c92e779795e0c413379aa5e0c468a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771174"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contentType = {
  contentType: 'https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101'
};

await client.api('/sites/id/lists/{list-id}/contentTypes/addCopy')
    .version('beta')
    .post(contentType);

```