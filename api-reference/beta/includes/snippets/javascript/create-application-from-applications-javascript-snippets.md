---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 562dccbb50af929f96d73927093b6371e13758d4
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "38000176"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  displayName: "Display name"
};

let res = await client.api('/applications')
    .version('beta')
    .post(application);

```