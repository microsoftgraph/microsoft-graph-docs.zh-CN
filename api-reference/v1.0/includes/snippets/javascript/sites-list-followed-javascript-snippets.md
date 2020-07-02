---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cdbbb60fe41438f19cb9b969be2719983421102
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006673"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/followedSites')
    .get();

```