---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16ee7b7e791abd8472c846200805dbdd186ef968
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473907"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sessions = await client.api('/communications/callRecords/{id}/sessions')
    .expand('segments')
    .get();

```