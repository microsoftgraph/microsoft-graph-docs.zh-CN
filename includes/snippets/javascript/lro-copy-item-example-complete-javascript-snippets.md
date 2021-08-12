---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e405ca8c4c36f178749ff7e4b3ae484a7680ad5a542eb6e7cfc5e7ede502299
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}')
    .version('beta')
    .get();

```