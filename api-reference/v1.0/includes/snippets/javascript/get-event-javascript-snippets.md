---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 225f7a97f633aef88facbf61789d868bf87b89ab5f183cbd5b1aa84be50630c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219362"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let event = await client.api('/me/events/AAMkAGIAAAoZDOFAAA=')
    .header('Prefer','outlook.timezone="Pacific Standard Time"')
    .select('subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees')
    .get();

```