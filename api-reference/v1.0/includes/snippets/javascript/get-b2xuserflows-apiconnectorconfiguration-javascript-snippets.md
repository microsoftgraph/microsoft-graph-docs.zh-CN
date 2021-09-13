---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10817862024dc9027f9011bf3a1c9364ac5a56984d241f30c496bf850bb01857
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332147"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userFlowApiConnectorConfiguration = await client.api('/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration')
    .expand('postAttributeCollection')
    .get();

```