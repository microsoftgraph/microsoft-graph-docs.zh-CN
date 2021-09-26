---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5869e0854684a4651f032219e5fd7d8df166eacfc2a372dd559d16596370924c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schemaExtensions = await client.api('/schemaExtensions')
    .version('beta')
    .filter('id eq \'graphlearn_test\'')
    .get();

```