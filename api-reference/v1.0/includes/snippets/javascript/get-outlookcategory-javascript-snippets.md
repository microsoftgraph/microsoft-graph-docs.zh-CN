---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81de791d1889f3af0fa8101ad4d9ffd0e085918ee25d478816c8a148d36141b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let outlookCategory = await client.api('/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7')
    .get();

```