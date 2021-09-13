---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0a1ac79e435df99de31ae2f30a5c1fed05998fc1af6188826c96b7c093ce9a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107108"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarGroup = await client.api('/me/calendarGroups/{id}')
    .get();

```