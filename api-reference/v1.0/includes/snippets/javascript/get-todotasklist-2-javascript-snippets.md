---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6650ba85064acc904740f50ef6b29d48d2ef192f37efe9f7674e17779a05d5ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903856"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let todoTaskList = await client.api('/me/todo/lists/AAMkADIyAAAAABrJAAA=')
    .get();

```