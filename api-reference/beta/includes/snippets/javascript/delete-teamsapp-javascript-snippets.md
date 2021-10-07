---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df843972b8f751c68970dad90f17054aac8cd6e5b53beb772135b187c0ade6d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332847"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8')
    .version('beta')
    .delete();

```