---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ad5fd606d3c4cf3a12b40a7530c5edb9dbc48e699c0b2bcb2c3cf3f66635918
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106189"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let events = await client.api('/me/calendar/events')
    .version('beta')
    .get();

```