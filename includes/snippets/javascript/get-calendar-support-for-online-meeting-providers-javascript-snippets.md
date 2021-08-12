---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0510e998e73fda3ab420f6b211b920e88b8db5037ad647aa9143f7f8a808d9f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240540"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendar')
    .get();

```