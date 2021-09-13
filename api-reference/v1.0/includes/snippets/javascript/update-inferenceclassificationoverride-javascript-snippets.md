---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 808250f7dbbffe3043ea7e78da9763d56ef43da607e078e2a7b20539d2f40882
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278829"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const inferenceClassificationOverride = {
  classifyAs: 'focused'
};

await client.api('/me/inferenceClassification/overrides/{id}')
    .update(inferenceClassificationOverride);

```