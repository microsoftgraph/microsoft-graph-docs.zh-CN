---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b3794520372aa14e295cbb0646463263d733b93
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/mentions/{id}')
    .version('beta')
    .delete();

```