---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3a4e162563c7e5465641a69b741c40a4bfb3ab5
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428787"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

let res = await client.api('/me/getMemberObjects')
    .post(string);

```