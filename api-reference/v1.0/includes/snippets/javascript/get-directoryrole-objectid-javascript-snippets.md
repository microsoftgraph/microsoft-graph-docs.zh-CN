---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f01f323c02863d097110e09117bfaad244ad1251a4d0f9161586ada310887942
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277682"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRole = await client.api('/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda')
    .get();

```