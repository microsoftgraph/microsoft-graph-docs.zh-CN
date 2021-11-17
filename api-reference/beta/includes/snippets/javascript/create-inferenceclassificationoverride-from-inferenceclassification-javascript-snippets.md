---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 544c91cdf6e7d1ddaf9dfc727acb4cbd20126531269c5b1e75520a2a6b951610
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333025"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const inferenceClassificationOverride = {
  classifyAs: 'focused',
  senderEmailAddress: {
    name: 'Samantha Booth',
    address: 'samanthab@adatum.onmicrosoft.com'
  }
};

await client.api('/me/inferenceClassification/overrides')
    .version('beta')
    .post(inferenceClassificationOverride);

```