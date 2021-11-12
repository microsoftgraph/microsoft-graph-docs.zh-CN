---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04992fb3ac4ac21bdf493cd90eb2e5bc76475756399fcd4b81d7f0d881373283
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106178"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/me/contactFolders/{id}/contacts')
    .version('beta')
    .get();

```