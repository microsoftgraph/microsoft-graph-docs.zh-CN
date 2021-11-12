---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9abf2243a7ef5c4cfd7414a420f8b7d03914d476476c1ca0f0373167fc4eed6a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158552"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let domains = await client.api('/domains')
    .version('beta')
    .get();

```