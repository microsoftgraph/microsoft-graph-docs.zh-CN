---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fc4e909308fbaeb9b0a4d8cab59cc24a0c5a683f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890821"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/delta')
    .get();

```