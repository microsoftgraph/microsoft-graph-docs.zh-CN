---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 625540c8d0efd774606dd746b410b68c93324f49
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771251"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let shiftPreferences = await client.api('/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences')
    .get();

```