---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfdd664eac161965dee0f986bc0640807ff68935
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274770"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11012/assignments/19002/getResourcesFolderUrl')
    .version('beta')
    .get();

```