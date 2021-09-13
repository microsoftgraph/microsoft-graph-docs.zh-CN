---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33b8d72566901b8aa970a04e7ff20a6f476535fc9581a88bb1da7f07e7605f77
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409582"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsTab = await client.api('/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d')
    .expand('teamsApp')
    .get();

```