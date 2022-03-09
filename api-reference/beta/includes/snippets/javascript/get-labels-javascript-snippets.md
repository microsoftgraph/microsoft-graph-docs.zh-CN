---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a8ca6f89aee8b6d36f9b7a83cb77ef8ee782cd1137bf9843640b79e5bcad392
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278463"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let labels = await client.api('/me/informationProtection/policy/labels')
    .version('beta')
    .get();

```