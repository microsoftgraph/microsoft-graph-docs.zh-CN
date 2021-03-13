---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 502cc3fcfb0e1926bd421ef32ea293e2828d553a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806141"
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