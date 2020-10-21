---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c4423886deb4a3512695a3629b5fd0c8d80ca84
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610738"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders')
    .get();

```