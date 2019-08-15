---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 335af084e525ec130e9c6390ec187c70131521c4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408436"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const agreement = {
  displayName: "displayName-value",
  isViewingBeforeAcceptanceRequired: true
};

let res = await client.api('/agreements/{id}')
    .version('beta')
    .update({agreement : agreement});

```