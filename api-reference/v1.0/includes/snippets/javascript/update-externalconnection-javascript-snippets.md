---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ea8f7a2e05c04bc4da18e4e3532975e4c43525acc505f14ffefc743d589a633
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378780"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalConnection = {
  name: 'Contoso HR Service Tickets',
  description: 'Connection to index HR service tickets'
};

await client.api('/connections/contosohr')
    .update(externalConnection);

```