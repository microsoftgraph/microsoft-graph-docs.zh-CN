---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ef755c36b18f17c90892e9880177c2cae11516a9926124e7d2afdd8b22fd28e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendar/events/AAMkADJXJGu0AABf02qwAAA=')
    .get();

```