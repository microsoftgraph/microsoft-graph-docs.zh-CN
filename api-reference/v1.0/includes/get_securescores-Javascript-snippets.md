---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2759a65cba2c5917bf42262886c0a50d7c89f47c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481455"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/secureScores')
    .top(1)
    .get();

```