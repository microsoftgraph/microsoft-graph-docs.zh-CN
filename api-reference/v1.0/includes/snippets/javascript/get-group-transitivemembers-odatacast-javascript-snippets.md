---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e08fe0b03f8c4073d0731af1767368adf9c8fbc99551336361baa80daa07b4d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328962"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/groups/{id}/transitivemembers/microsoft.graph.group')
    .header('ConsistencyLevel','eventual')
    .get();

```