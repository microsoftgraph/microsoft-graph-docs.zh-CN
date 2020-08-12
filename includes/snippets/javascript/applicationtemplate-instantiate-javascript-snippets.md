---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9228257d39e49e01c95fefd59808d2b9864d70c
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const applicationServicePrincipal = {
  displayName: "AWS Contoso"
};

let res = await client.api('/applicationTemplates/8b1025e4-1dd2-430b-a150-2ef79cd700f5/instantiate')
    .version('beta')
    .post(applicationServicePrincipal);

```