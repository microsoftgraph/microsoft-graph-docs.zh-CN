---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 093230e97be2c74eadf3fdb7289a869dbbe42ac685fcfefa99dee5b5ef792a54
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162221"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appRoleAssignments = await client.api('/groups/7679d9a4-2323-44cd-b5c2-673ec88d8b12/appRoleAssignments')
    .version('beta')
    .get();

```