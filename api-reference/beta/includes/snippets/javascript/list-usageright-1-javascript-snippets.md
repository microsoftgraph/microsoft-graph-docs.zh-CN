---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09ddb6b5e480060790f81fae0207f80abc9d12531ccb616b994c95242ae5c7f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106921"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let usageRights = await client.api('/devices/{objectId}/usageRights')
    .version('beta')
    .get();

```