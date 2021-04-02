---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43ebeba990955a66630d7689b4a50881b3eb9469
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507159"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/termStore/groups/{groupId}')
    .version('beta')
    .get();

```