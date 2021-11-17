---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75eb313d09441b4f9c58d6e5baaa9afd45dc530aa5d08e09c989215ed024244b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278898"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/skills/{id}')
    .version('beta')
    .delete();

```