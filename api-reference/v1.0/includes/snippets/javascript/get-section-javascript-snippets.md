---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7aa062dcfa81773b4d938b0e0dd7fcda93f5b90ba5e089428cfbec57f34af9f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105318"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onenoteSection = await client.api('/me/onenote/sections/{id}')
    .get();

```