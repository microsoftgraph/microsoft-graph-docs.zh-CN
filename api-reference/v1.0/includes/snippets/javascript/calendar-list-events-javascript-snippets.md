---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26e5eae400e3eebcf74ca7105d6035e093bc2578
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59997154"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let events = await client.api('/me/calendar/events')
    .filter('startsWith(subject,\'All\')')
    .get();

```