---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8215ef97eed4eb65c5a938f430c9cbcddf12db68
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636733"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: "Volunteer"
};

let res = await client.api('/me/calendars')
    .version('beta')
    .post(calendar);

```