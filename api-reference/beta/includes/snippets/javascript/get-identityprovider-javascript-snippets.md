---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 686e1c9307a7d3f33bdca2f2182cb0a8996236fc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805196"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviders = await client.api('/identityProviders')
    .version('beta')
    .get();

```