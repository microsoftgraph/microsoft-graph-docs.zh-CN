---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd4b36fc1f5275c6174a64fc7eeb09af10317ebaf315d1367fbf0cb0e99275dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333941"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let apiConnectors = await client.api('/identity/apiConnectors')
    .get();

```