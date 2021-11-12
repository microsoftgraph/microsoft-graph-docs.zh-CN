---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc0fc4203ccbd483558219ce7f94a757d6b43590a5d8e8eacfb02208269a6e8d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902243"
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

await client.api('/print/taskDefinitions/{printTaskDefinitionId}')
    .update(printTaskDefinition);

```