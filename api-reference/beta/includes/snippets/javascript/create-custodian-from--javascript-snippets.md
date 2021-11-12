---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7142a3c02176cd5e6b16fb215551c43f6d4b3e27369879ab7134bc988e7a9b95
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164001"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const custodian = {
    email: 'AdeleV@contoso.com',
    applyHoldToSources: 'true'
};

await client.api('/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians')
    .version('beta')
    .post(custodian);

```