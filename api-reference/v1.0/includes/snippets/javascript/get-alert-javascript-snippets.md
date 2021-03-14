---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0725c72f3a352919e57cf5fe0c744325e8e3ee86
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807508"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let alert = await client.api('/security/alerts/{alert_id}')
    .get();

```