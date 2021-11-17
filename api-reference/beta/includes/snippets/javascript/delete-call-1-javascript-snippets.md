---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 600ed8395e13d56c2421ed7ccc3985ca1e34c427a9f22628c559046d02b8fa9a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163719"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896')
    .version('beta')
    .delete();

```