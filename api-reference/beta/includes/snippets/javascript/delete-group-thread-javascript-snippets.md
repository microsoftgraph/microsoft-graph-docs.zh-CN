---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4eeb580ad81f79ebc5f63337808a5cdd7edbe18176175293b197b93c43f576d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215632"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==')
    .version('beta')
    .delete();

```