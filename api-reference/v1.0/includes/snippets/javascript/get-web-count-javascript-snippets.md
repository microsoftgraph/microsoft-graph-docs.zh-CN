---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9156804145498e7be562fe7f9ead783de2947e1f
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905586"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Web')
    .get();

```