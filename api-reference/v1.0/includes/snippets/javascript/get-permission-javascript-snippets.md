---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bf9703063130466d1bcd27754f67d80cca6ad6a
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176867"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .get();

```