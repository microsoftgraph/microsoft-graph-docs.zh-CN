---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5158a246729214a57bc6908c75ad70fc03ac86836f5ea712238823aea17f67f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104737"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskyUsers = await client.api('/riskyUsers')
    .version('beta')
    .get();

```