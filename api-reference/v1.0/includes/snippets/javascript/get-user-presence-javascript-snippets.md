---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 782ff6d9bcb6c4789d50943e753e7201b661fbb740ea09918dac01b4d34464bc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219314"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let presence = await client.api('/users/66825e03-7ef5-42da-9069-724602c31f6b/presence')
    .get();

```