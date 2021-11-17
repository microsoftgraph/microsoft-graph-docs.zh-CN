---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cbf6c27b2977869f0456ba9391d6468d90f7296
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "61021827"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getRecentNotebooks = await client.api('/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)')
    .version('beta')
    .get();

```