---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29992c62d99137b67db52825953372417bade8db
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774396"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11016/members')
    .version('beta')
    .get();

```