---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd85a63d128144f6ee92256df055feee70d0664adfb17b5b0fd285aaf6e911b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902631"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/accessReviews/definitions/filterByCurrentUser(on='reviewer')')
    .version('beta')
    .get();

```