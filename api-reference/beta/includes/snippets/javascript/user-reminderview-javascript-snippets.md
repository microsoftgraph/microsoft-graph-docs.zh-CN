---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 441b803cfecfe2d3c89a3d3f88a7b6aed6090151aea271f940717eab879bd97b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105696"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let reminderView = await client.api('/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')')
    .version('beta')
    .get();

```