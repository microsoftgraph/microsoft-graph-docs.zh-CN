---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f96f30c99412f890d3261b538e264a9fb79822816cf18cf0a096401d1f3329a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333166"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/en/defaultPages/idpselections/$value')
    .version('beta')
    .get();

```