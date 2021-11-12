---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2de0d4a0dd8b687640af6a0fcfb1aa5c62e396999f8b86204e102084b1c53d11
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216020"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskGroup = {
  name: 'Personal Tasks',
};

await client.api('/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=')
    .version('beta')
    .update(outlookTaskGroup);

```