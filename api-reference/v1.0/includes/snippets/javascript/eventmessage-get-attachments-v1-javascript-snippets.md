---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16a18afe30a3e4195dcfbbc9858cdb94aca96a48
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802796"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachments = await client.api('/me/messages/{id}/attachments')
    .get();

```