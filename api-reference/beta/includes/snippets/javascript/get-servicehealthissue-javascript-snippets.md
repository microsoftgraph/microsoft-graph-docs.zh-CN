---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 124beea002daa992536e944268df11fc5f9a11fa
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208994"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let serviceHealthIssue = await client.api('/admin/serviceAnnouncement/issues/MO226784')
    .version('beta')
    .get();

```