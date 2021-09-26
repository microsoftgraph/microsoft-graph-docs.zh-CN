---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b869149305dca460583e967c391a50a6c74ae6fda190bc4a4275f90f45b6817e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163909"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getEffectivePermissions = await client.api('/deviceManagement/virtualEndpoint/getEffectivePermissions')
    .version('beta')
    .get();

```