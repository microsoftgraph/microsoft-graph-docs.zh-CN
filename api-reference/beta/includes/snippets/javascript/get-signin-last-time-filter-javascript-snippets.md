---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d50fff0dbb8264e56562056149aafc1cd5353c7
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947177"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .version('beta')
    .filter('startswith(displayName,'Eric'),')
    .select('displayName,signInActivity')
    .get();

```