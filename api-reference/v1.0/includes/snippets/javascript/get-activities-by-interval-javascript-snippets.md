---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d1551e30eb22bd0ec7c53a14705a04d8dc8e576
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781776"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getActivitiesByInterval = await client.api('/drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')')
    .get();

```