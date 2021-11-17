---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9cb7b5ae05b8a3a7e183cdbba9740ad61df5a2a9c12e41d779abfb4f01c7940
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215656"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenLifetimePolicies = await client.api('/applications/{id}/tokenLifetimePolicies')
    .version('beta')
    .get();

```