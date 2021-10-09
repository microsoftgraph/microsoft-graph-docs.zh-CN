---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cbfac73894c701e1715b1216a6a7b11d55b94d787f61eac1b87f5a304543763
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278407"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRole = await client.api('/directoryRoles/roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b')
    .version('beta')
    .get();

```