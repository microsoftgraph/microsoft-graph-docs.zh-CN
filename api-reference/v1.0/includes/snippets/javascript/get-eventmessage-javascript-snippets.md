---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa4447a789bae552004c6c635f94910295253db9385798c1cf7043b2a468187a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409565"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AAMkADYAAAImV_lAAA=')
    .get();

```