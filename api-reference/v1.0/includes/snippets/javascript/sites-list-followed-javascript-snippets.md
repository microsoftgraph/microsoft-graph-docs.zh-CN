---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec1e8a4cefeab7fdda34c5360a117a23f487d25df2875854b9b2cad191d24976
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56831181"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let followedSites = await client.api('/me/followedSites')
    .get();

```