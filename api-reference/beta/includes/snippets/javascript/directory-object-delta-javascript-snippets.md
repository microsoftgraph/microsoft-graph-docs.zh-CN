---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 97a53a11800301d009a319a3f21235a02c77f20f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862441"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryObjects/delta')
    .version('beta')
    .get();

```