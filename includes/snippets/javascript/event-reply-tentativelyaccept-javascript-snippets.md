---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3381b831ad55a414e6c487555de82ec22d79e226432792a16cee332bf2eb47dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129771"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tentativelyAccept = {
  comment: "I will probably be able to make it.",
  sendResponse: true
};

let res = await client.api('/me/events/AAMkADADVj3fyAABZ5ieyAAA=/tentativelyAccept')
    .post(tentativelyAccept);

```