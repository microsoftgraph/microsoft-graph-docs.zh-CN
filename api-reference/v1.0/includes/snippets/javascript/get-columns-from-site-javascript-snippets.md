---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55c7673a1189fc4f695be0d0c3e6d78bc3f57c45
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021999"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columns = await client.api('/sites/{site-id}/columns')
    .get();

```