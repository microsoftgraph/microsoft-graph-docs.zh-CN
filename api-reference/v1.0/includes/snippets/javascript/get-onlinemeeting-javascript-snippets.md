---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 799195d4e8407302fc6ee2b3f2f3c6e450e92f13
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803428"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onlineMeetings = await client.api('/communications/onlineMeetings/')
    .filter('VideoTeleconferenceId eq \'123456789\'')
    .get();

```