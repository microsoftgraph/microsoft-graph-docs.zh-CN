---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d61b551332dfa48235d70fa641c8f1715d2d2c5bad54d0cfad31923f96fe9ef6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106786"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let extension = await client.api('/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions/Com.Contoso.Deal/')
    .get();

```