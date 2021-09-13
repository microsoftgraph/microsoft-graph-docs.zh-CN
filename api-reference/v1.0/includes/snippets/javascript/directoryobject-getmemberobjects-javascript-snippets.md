---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e401c173b8b5f2921d811c5cfa89acffadfa7e25d9f38f6eac5077226af6287b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277892"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/directoryObjects/{object-id}/getMemberObjects')
    .post(string);

```