---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 562dccbb50af929f96d73927093b6371e13758d4
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
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