---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d9ce0c07b0a5efcb2215d22e7ad1e6530c70cd0
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368880"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let posts = await client.api('/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/threads/AAQkADI5YzgxODgyLTExZDgtNDhkMS1iZDRjLTBhZGZiN2ExYWQxNwMkABAADW7fw6FZNEuyjrGA9R8SshAADW7fw6FZNEuyjrGA9R8Ssg==/posts')
    .get();

```