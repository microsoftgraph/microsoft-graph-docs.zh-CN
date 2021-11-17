---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fbb745a6929e4bb5bb0535db7bfd9c92369fd25d1310e78305836df8533d4a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105711"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groups = await client.api('/termStore/groups')
    .version('beta')
    .get();

```