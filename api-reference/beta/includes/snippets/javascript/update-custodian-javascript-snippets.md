---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53ab655bdcb1e63b594d1994919250f8e1697d0d4814289288b75b8bd091b107
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278395"
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