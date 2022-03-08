---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f49cbe54b555d2ee193df2cce4a7a3f336b2774f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338396"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let qnas = await client.api('/search/qnas')
    .version('beta')
    .get();

```