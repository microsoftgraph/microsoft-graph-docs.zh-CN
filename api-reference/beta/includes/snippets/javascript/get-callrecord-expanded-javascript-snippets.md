---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0ecf5f312082f9e692e21cdb843bdab79a5a6cc
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472600"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let callRecord = await client.api('/communications/callRecords/{id}')
    .version('beta')
    .expand('sessions($expand=segments)')
    .get();

```