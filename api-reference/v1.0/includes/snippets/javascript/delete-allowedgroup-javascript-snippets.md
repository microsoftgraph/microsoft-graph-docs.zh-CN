---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d8dd1f977f45c2025cf154db17be9760c5e4fa7b3192a24880a17162391e262
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333351"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/shares/{printerShareId}/allowedGroups/{groupId}/$ref')
    .delete();

```