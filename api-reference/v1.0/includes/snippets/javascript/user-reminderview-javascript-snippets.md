---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b7c2e3f1c864f42bf3c38e2f7e2d79ea8629e4d97cfb87a8df9552eaedcf22e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903200"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let reminderView = await client.api('/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')')
    .get();

```