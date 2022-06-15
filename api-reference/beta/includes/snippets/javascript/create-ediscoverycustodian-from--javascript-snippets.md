---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 586beb723b2ed066ce1ef151c76cd6e919aab518
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093489"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ediscoveryCustodian = {
    email: 'AdeleV@contoso.com',
};

await client.api('/security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians')
    .version('beta')
    .post(ediscoveryCustodian);

```