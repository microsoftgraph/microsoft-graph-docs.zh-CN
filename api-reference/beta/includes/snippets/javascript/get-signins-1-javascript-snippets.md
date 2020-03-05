---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27ec6610634a2266c765361183657e87a9c1874d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997553"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs/signIns')
    .version('beta')
    .get();

```