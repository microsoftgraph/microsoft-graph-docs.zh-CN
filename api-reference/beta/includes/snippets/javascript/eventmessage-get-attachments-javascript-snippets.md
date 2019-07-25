---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 758d38b9464102ebdfbc425c272494c87398a498
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859300"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/attachments')
    .version('beta')
    .get();

```