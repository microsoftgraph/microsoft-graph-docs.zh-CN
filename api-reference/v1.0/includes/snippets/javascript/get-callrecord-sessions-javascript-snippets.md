---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5407767331ce35d60f700a0e83c415096911e449a38ade70fc527b491fafbbda
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333247"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sessions = await client.api('/communications/callRecords/{id}/sessions')
    .get();

```