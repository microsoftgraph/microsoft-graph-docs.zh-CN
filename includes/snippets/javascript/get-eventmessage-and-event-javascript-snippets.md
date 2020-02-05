---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a45b31d4d7410ecee720e9a692483ad9274398e
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774636"
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