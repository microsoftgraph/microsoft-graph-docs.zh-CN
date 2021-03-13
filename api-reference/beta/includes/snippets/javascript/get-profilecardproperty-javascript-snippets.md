---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca45d83541ab9d0297c6d31e3c235517347670c8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785738"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let profileCardProperty = await client.api('/organization/{organizationId}/settings/profileCardProperties/{id}')
    .version('beta')
    .get();

```