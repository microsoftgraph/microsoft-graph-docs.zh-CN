---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5789f4ad107390e90b96b98d267a14c9f73018f3427c6e3e647c2ab0ebd58774
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220073"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/security/securityActions/{id}/cancelSecurityAction')
    .version('beta')
    .post();

```