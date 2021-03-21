---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b07ca951d7d9e1566b1099e76e123b43a9a3af5a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955215"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let defaultPages = await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/en/defaultPages')
    .version('beta')
    .get();

```