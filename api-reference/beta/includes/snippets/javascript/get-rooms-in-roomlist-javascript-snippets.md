---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 119441b1b59c2db0d6eb3b8fabc8236cb48c1518
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876756"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms')
    .version('beta')
    .get();

```