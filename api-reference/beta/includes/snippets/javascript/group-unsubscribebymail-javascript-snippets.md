---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21c3454b6718c909abfee1c49d23cde556e906c90a5cffee05248c17c7cdb6aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219036"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/unsubscribeByMail')
    .version('beta')
    .post();

```