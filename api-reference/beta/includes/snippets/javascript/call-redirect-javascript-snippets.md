---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7b60c7f2d15c709631261175ca76f85effd91d54
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708793"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const redirect = {
  targets: [
    {
      endpointType: "default",
      identity: {
        user: {
          id: "550fae72-d251-43ec-868c-373732c2704f",
          tenantId: "72f988bf-86f1-41af-91ab-2d7cd011db47",
          displayName: "Heidi Steen"
        }
      },
      languageId: "en-US",
      region: "westus"
    }
  ],
  targetDisposition: "default",
  timeout: 99,
  maskCallee: false,
  maskCaller: false
};

let res = await client.api('/app/calls/{id}/redirect')
    .version('beta')
    .post(redirect);

```