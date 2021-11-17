---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b444b85675b52e2547a06d51c45af929ef0ce41ef43071707afe4e19b51002cc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902527"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let alerts = await client.api('/security/alerts')
    .version('beta')
    .get();

```