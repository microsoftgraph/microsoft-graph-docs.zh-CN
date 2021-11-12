---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8b026b1e3a8c8a9b6956aa9af7cd9246d97a72eb88f4d6ba45da657e98c3bfa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277300"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let taskGroups = await client.api('/me/outlook/taskGroups')
    .version('beta')
    .get();

```