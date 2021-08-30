---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae6cd6edaabff5112f535ade1f7636ae1632fec4944bbd33fadd3062056b07e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161289"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversationMember = await client.api('/chats/19:b8577894a63548969c5c92bb9c80c5e1@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzJjOGQyYjVjLTE4NDktNDA2Ni1iNTdkLWU3YTBlOWU0NGVjOA==')
    .version('beta')
    .get();

```