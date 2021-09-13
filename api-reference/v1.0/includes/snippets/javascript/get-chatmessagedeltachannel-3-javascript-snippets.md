---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93114e4bf9de8189f3cf2395cc530aff0e272849aacfae3d314daa92fee8dd0a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221459"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta')
    .skiptoken('8UusBixEHS9UUau6uGcryrA6FpnWwMJbuTYILM1PArHxnZzDVcsHQrijNzCyIVeEauMQsKUfMhNjLWFs1o4sBS_LofJ7xMftZUfec_pijuT6cAk5ugcWCca9RCjK7iVj.DKZ9w4bX9vCR7Sj9P0_qxjLAAPiEZgxlOxxmCLMzHJ4')
    .get();

```