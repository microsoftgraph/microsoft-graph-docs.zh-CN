---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c50cba850707e2ab25c44f1661eee2f24633168775cab10fc9423bcb79542a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279747"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/accessReviews/definitions/3856fd6f-36e2-4152-97c9-76070d19f730')
    .delete();

```