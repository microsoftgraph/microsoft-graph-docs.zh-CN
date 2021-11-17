---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a5ce4024a300929ae4cea485997c17d1a178f157c66b2a8582d2bdab4111ddc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106343"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/messages/{id}')
    .version('beta')
    .delete();

```