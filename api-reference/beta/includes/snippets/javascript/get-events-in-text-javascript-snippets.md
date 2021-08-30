---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fd6361530547fca7428f57b5d537f38eba40e41a893f4eb23e31712d22dea1d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164062"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let events = await client.api('/me/events')
    .version('beta')
    .header('Prefer','outlook.body-content-type="text"')
    .select('subject,body,bodyPreview')
    .get();

```