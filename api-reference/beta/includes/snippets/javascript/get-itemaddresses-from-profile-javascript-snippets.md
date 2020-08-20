---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: baa25bd222a231b43b31ab7bbeaa2e5bd02c2891
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819493"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/addresses')
    .version('beta')
    .get();

```