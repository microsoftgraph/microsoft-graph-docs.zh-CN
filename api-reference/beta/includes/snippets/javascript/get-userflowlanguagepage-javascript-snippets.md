---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a289581cf735e1f95a82945122bec6cc33b7464d
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179315"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/en/defaultPages')
    .version('beta')
    .get();

```