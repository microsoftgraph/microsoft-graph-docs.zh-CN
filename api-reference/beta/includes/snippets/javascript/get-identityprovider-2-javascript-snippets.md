---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7725e9998d54f8cec9de08b7f458655a6d25861
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961043"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProvider = await client.api('/identityProviders/{id}')
    .version('beta')
    .get();

```