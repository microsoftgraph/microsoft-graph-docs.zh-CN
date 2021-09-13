---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e4ed60b63fcc75f6dcf788c2cc4b2d3dd05c1a3221c938b070569025a4284d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902321"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/drives/{drive-id}')
    .get();

```