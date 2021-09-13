---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d77d41ce95a6641031ea1d39033b4a941b48ecbacb6724744548e1c576956c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163537"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/accessReviews/definitions/filterByCurrentUser(on='reviewer')')
    .get();

```