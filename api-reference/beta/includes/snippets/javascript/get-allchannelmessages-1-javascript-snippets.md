---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6918db82e41ec1edd0c86c56ce24f306378b48a4ec69970e42d0099ebede6d64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106947"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getAllMessages = await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/getAllMessages')
    .version('beta')
    .get();

```