---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 397aea3ee450776e0759c3737d9a30e9aa1996ff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775435"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const synchronizationTemplate = {
    id: 'SCIM-Test1',
    applicationId: '{id}',
    factoryTag: 'CustomSCIM'
};

await client.api('/applications/{id}/synchronization/templates')
    .version('beta')
    .post(synchronizationTemplate);

```