---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f884d2a0b11fef50bcb514e46cfd9b7ce071afc7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let shiftPreferences = await client.api('/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences')
    .version('beta')
    .get();

```