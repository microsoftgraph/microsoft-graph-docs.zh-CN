---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72d8ac70e54640dd529e34c195a13dee6264d01e62329ab0c4790aecc6877e39
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277231"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/education/schools/{school-id}/users')
    .get();

```