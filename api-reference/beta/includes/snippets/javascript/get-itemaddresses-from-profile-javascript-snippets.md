---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33c31fac1bd4ad2f71e83641a662025af0c03d0ad5114d0c0af376d0de65e959
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163791"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let addresses = await client.api('/me/profile/addresses')
    .version('beta')
    .get();

```