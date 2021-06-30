---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51782c06fddc8ac1c2b5ca5343efb63af82a3757
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210738"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let serviceHealth = await client.api('/admin/serviceAnnouncement/healthOverviews/Microsoft 365 suite')
    .version('beta')
    .expand('issues')
    .get();

```