---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96dff4c3c89320bef9febde72aed0432a3504434
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881372"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/{id}/childFolders')
    .get();

```