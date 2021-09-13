---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d05e2615bed183df8af9c8390d3e94257d6873ae16d3498fe5c9fd0fd116dc4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164090"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{userId}/profile/notes/{id}')
    .version('beta')
    .delete();

```