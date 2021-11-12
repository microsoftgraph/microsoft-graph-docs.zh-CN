---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96f41d134c49a5c8d41c126ff3ca617d0e5cbf210f1080f886c288d1cff54b31
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221125"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const legalHold = {
  description: 'This is a description for a legalHold'
};

await client.api('/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}')
    .version('beta')
    .update(legalHold);

```