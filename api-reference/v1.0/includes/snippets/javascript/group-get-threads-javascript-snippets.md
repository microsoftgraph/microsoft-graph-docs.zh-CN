---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a5e25deec84f12550f34afd0ce21163919e63d081fb015a817df1a1d7104cb4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277671"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threads = await client.api('/groups/{id}/threads')
    .get();

```