---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 050789f373a0c3c1a7d3de0ff32d7a99b417539ad4798b3bdfe43819d88bc0ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904016"
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