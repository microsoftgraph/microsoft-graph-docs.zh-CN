---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2f1d6d2504a4c94a315ff6a87181664a77bfa33
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997871"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/websites')
    .version('beta')
    .get();

```