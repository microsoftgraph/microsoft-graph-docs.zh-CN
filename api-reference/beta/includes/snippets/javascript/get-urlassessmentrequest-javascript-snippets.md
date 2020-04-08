---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44e9ee486c03606040628220ecfe4854ec288f88
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "40867155"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/informationProtection/threatAssessmentRequests/723c35be-8b5a-47ae-29c0-08d76ddb7f5b')
    .version('beta')
    .get();

```