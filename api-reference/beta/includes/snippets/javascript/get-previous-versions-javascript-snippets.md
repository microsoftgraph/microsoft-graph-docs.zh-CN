---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74ebaaf587650297b84e0584d8b1a240c1ae6aa9771837a708e69aceca557dac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163824"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let versions = await client.api('/me/drive/items/{item-id}/versions')
    .version('beta')
    .get();

```