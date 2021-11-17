---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fd1b6b216dd816972b1e6824f3dcea03f40bc1048014ac04d4703be998aa111
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219643"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMemberOf = await client.api('/groups/{id}/transitiveMemberOf')
    .get();

```