---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5661385e2c7644985d0f7133d8ff7d961afdcda3f1aa1b8a1cff7e4049fecc1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902969"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversation = await client.api('/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=')
    .get();

```