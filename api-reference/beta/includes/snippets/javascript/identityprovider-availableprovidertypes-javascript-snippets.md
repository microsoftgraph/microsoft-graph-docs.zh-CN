---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17059ab9c1f2b7848a9b36e29c2e551a90fbbefd2713fd92a1194088973df3bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104387"
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