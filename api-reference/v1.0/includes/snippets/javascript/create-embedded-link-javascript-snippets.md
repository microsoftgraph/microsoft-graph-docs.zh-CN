---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78cef8c359702eb1b9f40195e2a681a4acab4bfe2cbdf0e951f281df44ce7342
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107063"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: 'embed'
};

await client.api('/me/drive/items/{item-id}/createLink')
    .post(permission);

```