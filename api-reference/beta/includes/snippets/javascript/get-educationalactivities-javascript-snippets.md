---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d671903e801d7fd9e84bb0fac478401d63d885605105ed1a735f29fe37274529
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273850"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationalActivities = await client.api('/me/profile/educationalActivities')
    .version('beta')
    .get();

```