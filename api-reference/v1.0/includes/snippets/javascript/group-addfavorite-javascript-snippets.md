---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cb56201210cc8860e81975099be35039c18135953b84605de02a95d9e5f8c88
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378777"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/addFavorite')
    .post();

```