---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7569db6426a2e0161ec0ea8a46f48f53db6e944
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509853"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/oauth2permissiongrants/delta')
    .get();

```