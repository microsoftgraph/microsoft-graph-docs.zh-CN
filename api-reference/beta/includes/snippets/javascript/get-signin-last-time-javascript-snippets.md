---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ae4bb1cb1d72b4196339b940eccfdddbf05c3366a6cb65eb27d00ea4f7fd2b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378589"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .version('beta')
    .select('displayName,userPrincipalName,signInActivity')
    .get();

```