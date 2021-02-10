---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a78652f88077784fc7db81431e53b5b3b4388f40
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176468"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{sitesId}/permissions')
    .version('beta')
    .get();

```