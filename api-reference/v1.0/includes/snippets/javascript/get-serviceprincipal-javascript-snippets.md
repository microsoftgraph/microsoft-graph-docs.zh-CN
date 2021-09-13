---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a9e4b25cb1c9abc32ae1062efc591249ef019b51a5b2737bafc8b1f814cf29b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106416"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipal = await client.api('/servicePrincipals/{id}')
    .get();

```