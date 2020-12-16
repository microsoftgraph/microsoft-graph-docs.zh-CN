---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1524720614e4197e167d19c6cca791c7b64dcd9
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692671"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _case = {
  displayName: "My Case 1 - Renamed",
  description: "Updated description",
  externalId: "Updated externalId"
};

let res = await client.api('/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583')
    .version('beta')
    .update(_case);

```