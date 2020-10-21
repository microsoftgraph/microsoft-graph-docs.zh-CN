---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6eae99e66da1b1b0416a1f7772ae0886d74303ae
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607614"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}')
    .get();

```