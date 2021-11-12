---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9fc2e026cbcaf66068101bfe1b4bbb21d192dc507db10c1e8a342f5282ff826
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278102"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let owners = await client.api('/groups/{id}/owners')
    .version('beta')
    .get();

```