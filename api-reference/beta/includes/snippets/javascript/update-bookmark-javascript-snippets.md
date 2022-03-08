---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6ef63dc18fd5a15d6b0c3bbb61221ac0bf3e6c4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookmark = {
  description: 'Book a fancy vacation in Tuscany or browse museums in Florence.'
};

await client.api('/search/bookmarks/{bookmarksId}')
    .version('beta')
    .update(bookmark);

```