---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e717736eb8a63e101f9308f497a77cfc90f4f6a5
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774630"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendars')
    .get();

```