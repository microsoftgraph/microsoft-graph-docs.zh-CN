---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f903c8b3d202e42ab9833f33e9ed57c7f820e112
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074475"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let device = await client.api('/devices/000005c3-b7a6-4c61-89fc-80bf5ccfc366')
    .get();

```