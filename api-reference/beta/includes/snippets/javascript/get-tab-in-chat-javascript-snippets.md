---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37b2c381c269c5abb746b26b1fef663a6002bae69ed200248d1c6936a528565c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164014"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsTab = await client.api('/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d')
    .version('beta')
    .expand('teamsApp')
    .get();

```