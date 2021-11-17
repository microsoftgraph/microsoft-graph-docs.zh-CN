---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f13e84543976e9eeb1934ff963d2f80d5e944741fed503ea46ba39943b175ad3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902926"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachment = await client.api('/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=')
    .version('beta')
    .get();

```