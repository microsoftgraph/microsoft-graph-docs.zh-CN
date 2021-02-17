---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56b345ca2134aef1c710515c0fcf46ca0a534ff4
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274967"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2xUserFlows/B2X_1_PartnerSignUp/languages')
    .version('beta')
    .get();

```