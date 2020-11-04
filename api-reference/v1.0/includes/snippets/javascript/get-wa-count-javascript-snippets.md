---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f7d5504601b28cbdb57c8fa7914e715e725c38f
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905692"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .header('ConsistencyLevel','eventual')
    .search('displayName:wa')
    .orderby('displayName ')
    .get();

```