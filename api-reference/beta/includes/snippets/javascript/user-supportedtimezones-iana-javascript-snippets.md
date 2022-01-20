---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8cbf11d4313f221f46272b0c5f0b90f32fd3989c6480df9fb03d25d3059b303
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903504"
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