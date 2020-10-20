---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46441219b5773b9cce9aa76aa37e89c80b3a00c3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612016"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/shares/{shareIdOrEncodedSharingUrl}')
    .version('beta')
    .get();

```