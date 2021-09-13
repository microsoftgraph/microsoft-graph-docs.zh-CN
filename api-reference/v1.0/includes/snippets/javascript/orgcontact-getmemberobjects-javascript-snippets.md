---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f0520fe1270381ef4e96674c744fc3b55480a49debd6a581c7c3a75ecf625e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279329"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: false
};

await client.api('/contacts/{id}/getMemberObjects')
    .post(string);

```