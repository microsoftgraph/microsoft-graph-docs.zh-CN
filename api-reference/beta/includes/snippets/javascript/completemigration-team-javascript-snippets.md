---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cd0dfd34e0da6518f8390172a5c88c5764b4ad2dc237e7224d7113054178d03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902476"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/completeMigration')
    .version('beta')
    .post();

```