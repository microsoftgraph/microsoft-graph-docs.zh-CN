---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07f0cbea1e9b58405fa9bafc5529ad4e8738fe7f
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903644"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .header('ConsistencyLevel','eventual')
    .filter('startswith(displayName,'a'),')
    .orderby('displayName ')
    .top(1)
    .get();

```