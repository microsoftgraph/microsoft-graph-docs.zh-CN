---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ffe3342d6cec2896012a3599f02844534f4079161572e4d7204be61a71b2a1e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129770"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendars')
    .get();

```