---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 570ced96b71d52fb9b4e3368ff8651eab374bde2
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration')
    .version('beta')
    .expand('postAttributeCollection')
    .get();

```