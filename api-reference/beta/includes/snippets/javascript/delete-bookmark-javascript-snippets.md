---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f97f05bd3420cb3b8d8ff11daec056284d2e00c0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338926"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/search/bookmarks/{bookmarkId}')
    .version('beta')
    .delete();

```