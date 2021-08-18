---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90831dfe9676b6f7fac26daa51e35fad3e24281cf43780c124081062fba370a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163128"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/contacts')
    .version('beta')
    .get();

```