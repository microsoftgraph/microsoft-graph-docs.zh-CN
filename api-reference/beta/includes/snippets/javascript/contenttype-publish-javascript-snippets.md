---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 719998cc2cc4a7ca282b929cf653043b1c804dcdb1390283bbc08bde42bfda79
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{siteId}/contentTypes/{contentTypeId}/publish')
    .version('beta')
    .post();

```