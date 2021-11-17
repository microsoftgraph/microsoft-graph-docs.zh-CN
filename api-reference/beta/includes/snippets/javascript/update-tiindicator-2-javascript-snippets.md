---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1fda0c8fd0c2f1354cceba00b52a2e3117958c4269e8ecee57b38a2b60445a81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220188"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tiIndicator = {
  additionalInformation: 'additionalInformation-after-update',
  confidence: 42,
  description: 'description-after-update',
};

await client.api('/security/tiIndicators/{id}')
    .version('beta')
    .update(tiIndicator);

```