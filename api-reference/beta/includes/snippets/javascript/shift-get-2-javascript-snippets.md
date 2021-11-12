---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b04bb0c5322d89514136d116070c92be31c3f79151d7e660b010b750cc45a506
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104705"
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