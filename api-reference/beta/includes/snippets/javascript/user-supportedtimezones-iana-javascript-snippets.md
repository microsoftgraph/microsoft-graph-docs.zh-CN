---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1e8507b9400c79cc10d9d5a522c78c1e3caa1ac
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808062"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let supportedTimeZones = await client.api('/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')')
    .version('beta')
    .get();

```