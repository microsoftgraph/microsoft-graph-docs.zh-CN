---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c55a4be6167795e194485c88ab052e46f0e3aa23cda5d7e57f200b7aaf016553
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let namedLocation = await client.api('/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959')
    .version('beta')
    .get();

```