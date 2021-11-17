---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46af557cb2a96ef2aef9b04f66f281423bc3c38f500729a9e41adcd03cbba61a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902721"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let reviewers = await client.api('/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers')
    .version('beta')
    .get();

```