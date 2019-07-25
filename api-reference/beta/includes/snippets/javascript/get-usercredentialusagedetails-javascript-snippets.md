---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e3dc8c72a8d293bc2532ffbe1bc6e51ee4843c08
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871198"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/userCredentialUsageDetails')
    .version('beta')
    .get();

```