---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8dfa9ff75cdf02d00542ce63a2588161f9968a65c19ba87c62ea5913f0ba048d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278885"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTaskList = {
  displayName: 'Travel items'
};

await client.api('/me/todo/lists')
    .version('beta')
    .post(todoTaskList);

```