---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d4077262008820623b6a32a277c6c4e632d6c88c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434862"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsDeviceUsageUserDetail(period='D7')')
    .get();

```