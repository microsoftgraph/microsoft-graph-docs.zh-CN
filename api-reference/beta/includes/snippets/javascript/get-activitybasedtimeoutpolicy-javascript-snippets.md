---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 356d5785dd622cb980464407884d46add52c823a0a7caca3e204801131ffc2aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902610"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let activityBasedTimeoutPolicy = await client.api('/policies/activityBasedTimeoutPolicies/{id}')
    .version('beta')
    .get();

```