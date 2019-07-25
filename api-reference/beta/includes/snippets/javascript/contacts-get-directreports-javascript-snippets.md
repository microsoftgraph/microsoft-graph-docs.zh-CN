---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 205a1a9a89318febf27d65cf82a370569cdb31c2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877933"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/{id}/directReports')
    .version('beta')
    .get();

```