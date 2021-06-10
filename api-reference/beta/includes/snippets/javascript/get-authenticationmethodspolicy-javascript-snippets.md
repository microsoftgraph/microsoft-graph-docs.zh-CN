---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cac5fe542fd041263f4a2485264894ca8e70cc66
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869481"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodsPolicy = await client.api('/policies/authenticationMethodsPolicy')
    .version('beta')
    .get();

```