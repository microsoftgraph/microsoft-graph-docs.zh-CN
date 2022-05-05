---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1aea0188446fe986bcb3b016eeab26102b89bf98
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212139"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let internalDomainFederation = await client.api('/domains/contoso.com/federationConfiguration/6601d14b-d113-8f64-fda2-9b5ddda18ecc')
    .version('beta')
    .get();

```