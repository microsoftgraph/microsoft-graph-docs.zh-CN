---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c03eb6eed82af5d6f44020a364f3ae1650d9f9f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617294"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/sites')
    .version('beta')
    .get();

```