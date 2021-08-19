---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10a8ae712489e346ad9ae832dc0f64f1a71a390d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264197"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let serviceHealth = await client.api('/admin/serviceAnnouncement/healthOverviews/Microsoft 365 suite')
    .get();

```