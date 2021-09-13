---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8126aff19d13a1e16b3b2f9c4a4471f0b93a602857cb8e400586badd718ec2e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378454"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d')
    .delete();

```