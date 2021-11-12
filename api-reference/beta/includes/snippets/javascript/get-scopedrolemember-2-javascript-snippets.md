---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 108109c566366be28278f673ebe53cffc8af28f6bab61765f4c6269cde1bf040
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902569"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedRoleMembers = await client.api('/administrativeUnits/{id}/scopedRoleMembers')
    .version('beta')
    .get();

```