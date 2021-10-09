---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1797817f928738f9a0fb53fa6cd6b7bf3c7d870c10cb5fcd38dbd877486b05fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278405"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRole = await client.api('/directoryRoles/fe8f10bf-c9c2-47eb-95cb-c26cc85f1830')
    .version('beta')
    .get();

```