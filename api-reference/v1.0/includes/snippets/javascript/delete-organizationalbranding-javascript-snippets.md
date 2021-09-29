---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23903d9501a21bd6acbd3a08c814605330cf8c23
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995867"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/organization/84841066-274d-4ec0-a5c1-276be684bdd3/branding')
    .delete();

```