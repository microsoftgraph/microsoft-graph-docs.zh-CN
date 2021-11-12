---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 632901956164f157c25d8d68b3e2b1b22a75c951d9a01964220da8327e3963e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333092"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printTaskDefinition = {
  displayName: 'Test TaskDefinitionName',
  createdBy: {
    displayName: 'Requesting App Display Name'
  }
};

await client.api('/print/taskDefinitions')
    .version('beta')
    .post(printTaskDefinition);

```