---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1117231d321c6c18b24e46aafffa501b86a8a5db
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507497"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oauth2PermissionGrants = await client.api('/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/oauth2PermissionGrants')
    .get();

```