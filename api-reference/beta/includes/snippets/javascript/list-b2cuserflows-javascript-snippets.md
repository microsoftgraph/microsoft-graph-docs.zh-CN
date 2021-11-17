---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc1837cef6f6956f93072b763a74accae4bf34f461306f1972b42139282b0463
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163812"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2cUserFlows = await client.api('/identity/b2cUserFlows')
    .version('beta')
    .get();

```