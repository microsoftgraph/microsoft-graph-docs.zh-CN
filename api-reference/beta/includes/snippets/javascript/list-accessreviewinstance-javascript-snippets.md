---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3031bf6f3c3891d85cdc22093ebd97f50c882281
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573131"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let instances = await client.api('/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances')
    .version('beta')
    .skip(0)
    .top(100)
    .get();

```