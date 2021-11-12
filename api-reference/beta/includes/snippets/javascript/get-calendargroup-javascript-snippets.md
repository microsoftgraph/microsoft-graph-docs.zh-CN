---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a28ef376b12245684196e169e973d8650a16e4ae42cecb738b5688f8da3f590c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904270"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarGroup = await client.api('/me/calendarGroups/{id}')
    .version('beta')
    .get();

```