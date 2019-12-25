---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb7e6835b69bd57dc63ee7a3deffe42aba30da8e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871132"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const changeScreenSharingRole = {
  role: "viewer"
};

let res = await client.api('/communications/calls/{id}/changeScreenSharingRole')
    .post(changeScreenSharingRole);

```