---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58d02b1836b5912bc5d676818bdbb2477b0383d9672d8cdb4a432cc0e27bb562
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277417"
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