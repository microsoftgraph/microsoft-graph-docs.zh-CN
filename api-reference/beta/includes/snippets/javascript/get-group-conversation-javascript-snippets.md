---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97233c7aad046c24e0c1ebde50aa3b42fd5631357b398aaf2e90bf47c0437b6c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219047"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversation = await client.api('/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=')
    .version('beta')
    .get();

```