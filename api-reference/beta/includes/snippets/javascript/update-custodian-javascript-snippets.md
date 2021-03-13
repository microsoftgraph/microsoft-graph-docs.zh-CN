---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba3536176c7759dd8bf529d578d47a5240ecf49f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773198"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const custodian = {
  applyHoldToSources: 'false',
};

await client.api('/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239')
    .version('beta')
    .update(custodian);

```