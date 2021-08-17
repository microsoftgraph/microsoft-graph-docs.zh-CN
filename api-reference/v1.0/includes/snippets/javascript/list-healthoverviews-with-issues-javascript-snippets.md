---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0be88400542381ed2eaf38ea1d051c653fafe203
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259124"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let healthOverviews = await client.api('/admin/serviceAnnouncement/healthOverviews')
    .expand('issues')
    .get();

```