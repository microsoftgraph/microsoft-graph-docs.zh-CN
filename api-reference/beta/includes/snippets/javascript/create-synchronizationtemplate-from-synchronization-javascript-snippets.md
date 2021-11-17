---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf828d88a7c27338745710988c2e76cb1e4b4dc69b4f63166efb30b3ce8de57a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158469"
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