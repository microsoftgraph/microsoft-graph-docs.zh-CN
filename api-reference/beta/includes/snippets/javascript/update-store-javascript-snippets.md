---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cc0fe1bfe5de656b6f48222580b2a5114c92014
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803374"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const store = {
  defaultLanguageTag: 'en-US'
};

await client.api('/termStore')
    .version('beta')
    .update(store);

```