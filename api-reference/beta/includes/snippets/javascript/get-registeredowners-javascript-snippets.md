---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aaa02c53b529e38b0db945fdca0a1d4ba6f303575683eddc0d3b99bb8e848686
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219778"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let registeredOwners = await client.api('/devices/{id}/registeredOwners')
    .version('beta')
    .get();

```