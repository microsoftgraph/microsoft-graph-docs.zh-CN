---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffab11357686e37a0128790a7513b281a6fa8503dd30e199192343c1a4351f9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903876"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onenoteOperation = await client.api('/me/onenote/operations/{id}')
    .get();

```