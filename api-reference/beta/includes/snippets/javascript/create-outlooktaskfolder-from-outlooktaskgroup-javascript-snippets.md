---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f42b1a668a13b349e067bb350b5402e99f62de5d08452f71b601dd8cb36e3bff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903956"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskFolder = {
  name: 'Cooking'
};

await client.api('/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=/taskfolders')
    .version('beta')
    .post(outlookTaskFolder);

```