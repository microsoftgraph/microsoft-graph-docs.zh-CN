---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a897981540a14686e1b08514875770deab2bf2c5
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208892"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let issues = await client.api('/admin/serviceAnnouncement/issues')
    .version('beta')
    .get();

```