---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f09494db874fecd41ab4d7c04e2bf35f52042916
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35318644"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/{id}/messages/{id}/hostedContents/{id}')
    .version('beta')
    .get();

```