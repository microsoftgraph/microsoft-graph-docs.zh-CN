---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 338ee7f30b90d6fe9bf697a1f6cfd38ca978191e904630b3b7a252ff1da61256
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sectionGroup = await client.api('/me/onenote/sectionGroups/{id}')
    .get();

```