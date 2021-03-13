---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fffb80d396e027788b5cc5a9f7a18a333b012f6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789761"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let profileCardProperties = await client.api('/organization/{organizationId}/settings/profileCardProperties')
    .version('beta')
    .get();

```