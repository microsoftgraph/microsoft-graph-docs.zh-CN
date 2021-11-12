---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc2309d308c278a2886294da927992d27c0c30734e2e6f43837976ba6e9b2abf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let owners = await client.api('/applications/{id}/owners')
    .version('beta')
    .get();

```