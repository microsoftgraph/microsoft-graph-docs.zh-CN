---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dace62fd8a169bdce26407f51bdbe9ef391ac1c20edb3d73cc8ef45d4f20b0c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105114"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let keySets = await client.api('/trustFramework/keySets')
    .version('beta')
    .get();

```