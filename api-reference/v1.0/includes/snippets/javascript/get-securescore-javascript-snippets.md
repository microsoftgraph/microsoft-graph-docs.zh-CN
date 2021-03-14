---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40c95ab66f5a63324f801be84cf818fb33dda138
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810150"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let secureScore = await client.api('/security/secureScores/{id}')
    .get();

```