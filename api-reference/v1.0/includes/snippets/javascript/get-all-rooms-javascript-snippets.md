---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61b898eb6ea6d87e310c804f200138129ed5ee2be06ae653124222468d2da7b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163842"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let room = await client.api('/places/microsoft.graph.room')
    .get();

```