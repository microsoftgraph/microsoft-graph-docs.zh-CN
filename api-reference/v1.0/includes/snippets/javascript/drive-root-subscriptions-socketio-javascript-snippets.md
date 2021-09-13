---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3108f3464e4c91f8587f125a5ab1d2dc6e978bc340a240b17edc72b4a9c6b8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333469"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscription = await client.api('/me/drive/root/subscriptions/socketIo')
    .get();

```