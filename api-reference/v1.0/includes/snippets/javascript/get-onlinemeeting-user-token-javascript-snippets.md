---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 227d55d4b472ca0f3929903f911204e5b5b4887a
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664977"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onlineMeeting = await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy')
    .version('beta')
    .get();

```