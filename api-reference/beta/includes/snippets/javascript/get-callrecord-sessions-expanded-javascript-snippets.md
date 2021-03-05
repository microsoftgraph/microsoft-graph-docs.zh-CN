---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fa24dd724c412ac4bad185052b6d9ae7a04c8e9
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472626"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sessions = await client.api('/communications/callRecords/{id}/sessions')
    .version('beta')
    .expand('segments')
    .get();

```