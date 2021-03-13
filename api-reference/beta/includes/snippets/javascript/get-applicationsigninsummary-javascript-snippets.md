---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 894a295382bd133482963d844501ebb33c773992
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804776"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getAzureADApplicationSignInSummary = await client.api('/reports/getAzureADApplicationSignInSummary(period='D7')')
    .version('beta')
    .get();

```