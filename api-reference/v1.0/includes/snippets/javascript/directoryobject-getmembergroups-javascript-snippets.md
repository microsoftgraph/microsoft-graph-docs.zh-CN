---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70ea20c66be057d2981db493b248c95d1d34ac77b1ff3c3e8f3d2609977b8549
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278708"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/directoryObjects/{object-id}/getMemberGroups')
    .post(string);

```