---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 105e201a0d28c20478213eb05906aab0c1fd59af
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808320"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let availableProviderTypes = await client.api('/identityProviders/availableProviderTypes')
    .version('beta')
    .get();

```