---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8e2a12544f9a71d416f2928ba6a873a420923dab
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636529"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const Stream = The contents of the file goes here.;

let res = await client.api('/me/drive/items/{item-id}/content')
    .version('beta')
    .put(Stream);

```