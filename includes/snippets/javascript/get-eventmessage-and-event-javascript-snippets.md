---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 974361e3236511025214be73f6b327bc108b1184f5d67540e90c99f9a0f944e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129774"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADADVj3fyAABZ5hYdAAA=')
    .expand('eventMessage/event')
    .get();

```