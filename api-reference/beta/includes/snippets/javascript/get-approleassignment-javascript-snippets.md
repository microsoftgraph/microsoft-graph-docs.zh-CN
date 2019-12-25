---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8a731c861339c7cc8bd633a45a799513a93d8a9
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868368"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/appRoleAssignedTo/{id}')
    .version('beta')
    .get();

```