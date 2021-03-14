---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92cc7203f5fbc72c70b1a7f00eb4c009fd020684
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810200"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/shifts/{shiftId}')
    .delete();

```