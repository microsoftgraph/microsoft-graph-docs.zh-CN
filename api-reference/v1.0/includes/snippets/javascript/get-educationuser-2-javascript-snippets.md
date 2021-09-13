---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cade9df2d792641f50277cc0528d3570d9824455bc3c4ece5c641db2d7629ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902971"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationUser = await client.api('/education/users/{user-id}')
    .get();

```