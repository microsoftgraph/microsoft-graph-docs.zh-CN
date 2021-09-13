---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32856a38407ed5e01131dbe9c90eea12d6b98cc73e8beeb3a5f38a8542b65fb6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218651"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissions = await client.api('/sites/{sitesId}/permissions')
    .get();

```