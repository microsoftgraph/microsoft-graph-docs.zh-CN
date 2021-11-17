---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bbcbae6230e97983c3bf55fa95c1025c9c0cef645bc83e8b4350e1a83790eda
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106650"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/removeFavorite')
    .version('beta')
    .post();

```