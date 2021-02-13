---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a1c672444ead1fa83d93a2355d87375e2356988
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179309"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/schools/{school-id}/classes')
    .get();

```