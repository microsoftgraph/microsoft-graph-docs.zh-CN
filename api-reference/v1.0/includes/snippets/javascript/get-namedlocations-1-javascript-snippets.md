---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b809d29682d9ad23c85cf6472632fabad38e3ca6c31fed7a4b02a04503c7355e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277250"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let namedLocations = await client.api('/identity/conditionalAccess/namedLocations')
    .get();

```