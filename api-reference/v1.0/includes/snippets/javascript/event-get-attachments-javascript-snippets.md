---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7fa1b9317c0a8cda7df79e540a345359e3df4a66
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887340"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}/attachments')
    .get();

```