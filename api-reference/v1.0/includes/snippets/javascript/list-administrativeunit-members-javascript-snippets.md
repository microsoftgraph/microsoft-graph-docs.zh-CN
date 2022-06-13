---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c449f5dc6472e7910c7f2e5d6c5e919e880c71f9
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040923"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/directory/administrativeUnits/c5729e7c-988e-417b-b287-14f5bd4711d8/members')
    .get();

```