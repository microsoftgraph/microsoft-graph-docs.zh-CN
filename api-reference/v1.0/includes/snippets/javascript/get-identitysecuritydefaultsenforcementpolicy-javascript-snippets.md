---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a37bb63f798c679f87ac75706ed708cf0cbef648f06492bd792ef926d8fa63b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278837"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identitySecurityDefaultsEnforcementPolicy = await client.api('/policies/identitySecurityDefaultsEnforcementPolicy')
    .get();

```