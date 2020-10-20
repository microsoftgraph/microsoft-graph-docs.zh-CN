---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efe03e7d495070275d9c085319cf3af5358c6e3b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606877"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADYAAAImV_lAAA=')
    .version('beta')
    .get();

```