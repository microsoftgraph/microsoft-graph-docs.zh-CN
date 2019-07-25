---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9b5ec9a3a26a6eaef217cf9ccffedb8707d5fc45
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855250"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/owners')
    .version('beta')
    .get();

```