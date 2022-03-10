---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0d6f6a74ff68daf85c78ed87e5c75451357ff10
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411911"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/settings/3c105fc3-2254-4861-9e2d-d59e2126f3ef')
    .version('beta')
    .delete();

```