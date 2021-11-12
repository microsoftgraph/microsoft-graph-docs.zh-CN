---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7401db4cdeb587024778b320e31d1866eb917e41b34a24f213dc8006558b621b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let serviceConfigurationRecords = await client.api('/domains/contoso.com/serviceConfigurationRecords')
    .version('beta')
    .get();

```