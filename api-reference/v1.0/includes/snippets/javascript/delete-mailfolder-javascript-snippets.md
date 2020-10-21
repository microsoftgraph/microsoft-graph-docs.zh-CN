---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9e00c07b8f657f4d3319a7ec62d1d52ac2eefe2
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618522"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/{id}')
    .delete();

```