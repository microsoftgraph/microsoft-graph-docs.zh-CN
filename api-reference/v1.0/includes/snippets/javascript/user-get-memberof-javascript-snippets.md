---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad619386e45e976e531b7bec7ac9f69b7070202d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884943"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/memberOf')
    .get();

```