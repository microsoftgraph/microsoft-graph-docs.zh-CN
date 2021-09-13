---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abaf4c0614bbbaedb1d6f427390b64facc752eb38bb2795daf20eb9e60f5833e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221192"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let events = await client.api('/me/calendar/events')
    .get();

```