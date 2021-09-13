---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ceb1151a5a34955a65ce4a40ee4ef6dcd3bf7db1aa9ed642cb12839aefe380f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220116"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps')
    .get();

```