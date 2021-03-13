---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2941f730891abd7c215fe3cbff6e72ea3d5cc55e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777094"
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