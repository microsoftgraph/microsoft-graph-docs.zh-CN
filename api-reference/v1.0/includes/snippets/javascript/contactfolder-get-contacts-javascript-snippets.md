---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 072dfb71034b8a31bb58629a81911b3791f6ef6a909e48a473591c93cc85555c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333544"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/me/contactFolders/{id}/contacts')
    .get();

```