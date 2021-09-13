---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e70a0048dd770b57367cba96a8ea2d33077bc849c4dd7e0bd2b69ed49c8cb3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904146"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959')
    .delete();

```