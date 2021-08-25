---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4a96ab32e647ac314dafd1107e1fb83f8dddcb176ceec1fae307983101885f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162409"
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