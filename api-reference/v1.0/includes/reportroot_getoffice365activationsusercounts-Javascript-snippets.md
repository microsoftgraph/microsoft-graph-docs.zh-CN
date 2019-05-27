---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 61026e3e16ac8832542c4028933d8aaf5414bf85
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463324"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActivationsUserCounts')
    .get();

```