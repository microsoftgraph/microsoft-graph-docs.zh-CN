---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ce414d96f30d29b958b13f261e757b88a733721
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797530"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const synchronizationTemplate = {
    id: 'Slack',
    applicationId: '{id}',
    factoryTag: 'CustomSCIM'
};

await client.api('/applications/{id}/synchronization/templates/{templateId}')
    .version('beta')
    .put(synchronizationTemplate);

```