---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f379e53ea78889d28ef1ff2031b40cbf9968911626e36180f044789a7e66a45
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903354"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{item-id}/follow')
    .post();

```