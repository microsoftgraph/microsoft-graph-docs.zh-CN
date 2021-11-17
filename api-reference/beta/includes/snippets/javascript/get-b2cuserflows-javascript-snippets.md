---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07ffc584c5f531fa5e845aeb4282a4ca858514308c2d38fe148796872ec87a47
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104494"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2cIdentityUserFlow = await client.api('/identity/b2cUserFlows/{id}')
    .version('beta')
    .get();

```