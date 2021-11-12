---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5719dbfa17a38fbe36630c45963344215c436c852f8005cd747fd9ba964d9d5d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163130"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let orgContact = await client.api('/contacts/{id}')
    .version('beta')
    .get();

```