---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 211d359dbbe0966c01b3bc2d441b00fa6b69848563cc7932183d9910f90450fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329080"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ownedObjects = await client.api('/servicePrincipals/{id}/ownedObjects')
    .get();

```