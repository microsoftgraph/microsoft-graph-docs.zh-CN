---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 954fab18ed9f33c5a959032926c801b6c900fcac6a1687f12c3a2adfbece8c37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904117"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sections = await client.api('/me/onenote/sections')
    .get();

```