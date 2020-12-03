---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe42a054168cc91dadb05a5d8314f465e8b58304
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522656"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/v1.0/directoryObjects/{user-id}"
};

let res = await client.api('/directoryRoles/roleTemplateId={role-templateId}/members/$ref')
    .post(directoryObject);

```