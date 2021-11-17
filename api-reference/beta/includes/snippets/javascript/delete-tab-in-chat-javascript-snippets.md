---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b626d548927ed4fc9d5ba1e0e3bdd196b40cb849aa6cf9ac60bd51622b3ccb07
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164213"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d')
    .version('beta')
    .delete();

```