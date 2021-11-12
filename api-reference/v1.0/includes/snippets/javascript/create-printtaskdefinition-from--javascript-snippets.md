---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 303213111839bf3cc579faecfb539cb33cc622ec863282144b622afb5ec3c283
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104949"
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
    .post(printTaskDefinition);

```