---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33be736d99f6ffd34537c9c03dfbdb8d472250964328b403ea35af0bdfd62d91
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104476"
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