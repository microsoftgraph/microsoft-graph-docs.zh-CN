---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ababb1c63ca0d16646748afb03477bf17424470f8311e4ecf25eb1c850a9fa1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104687"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let temporaryAccessPassMethods = await client.api('/me/authentication/temporaryAccessPassMethods')
    .version('beta')
    .get();

```