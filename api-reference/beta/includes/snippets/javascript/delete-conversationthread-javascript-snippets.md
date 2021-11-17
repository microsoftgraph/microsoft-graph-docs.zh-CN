---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 270d557e41a182b9d8f3311c56000da223b25e44609eec79f1d4aa0c4b195c9a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158556"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/threads/{id}')
    .version('beta')
    .delete();

```