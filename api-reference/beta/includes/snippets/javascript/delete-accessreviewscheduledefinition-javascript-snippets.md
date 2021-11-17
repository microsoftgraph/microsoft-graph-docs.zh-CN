---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3762c0214608b794b7253c8c74a41ba89e94d57d6d74316814cc663fe1531b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902633"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/accessReviews/definitions/29f2d16e-9ca6-4052-bbfe-802c48981fd8')
    .version('beta')
    .delete();

```