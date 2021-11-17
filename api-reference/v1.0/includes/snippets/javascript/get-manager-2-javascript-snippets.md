---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bbf48403c95e0d72f7bd857c0b470794d65c5e517027bd1fa59611614021277
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409460"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/users/{id|userPrincipalName}/manager')
    .get();

```