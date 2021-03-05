---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9143f94abaa8707cc24414f6df56c070d5d89849
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473978"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let callRecord = await client.api('/communications/callRecords/{id}')
    .expand('sessions($expand=segments)')
    .get();

```