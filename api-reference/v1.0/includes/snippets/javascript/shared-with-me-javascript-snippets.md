---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f0d13c781508ca5f0d1db64eeb2955bfe2b417e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614103"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/sharedWithMe')
    .get();

```