---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ec75e3d1a88990bc03b3865d93d2abc4c69a04b85ee5be70f0d060a0dabf087
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219472"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let shares = await client.api('/print/shares')
    .get();

```