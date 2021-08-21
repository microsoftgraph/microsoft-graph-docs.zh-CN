---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7836851cfeeb94c0028ec385d4cf23680ddb27c2879bfd3a4987cb16c38d852b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219856"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRoles = await client.api('/privilegedRoles')
    .version('beta')
    .get();

```