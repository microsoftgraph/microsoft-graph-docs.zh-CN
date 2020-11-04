---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37c5a8e3e9cdf7d02d68adec2f258187bffe3118
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905258"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Android')
    .get();

```