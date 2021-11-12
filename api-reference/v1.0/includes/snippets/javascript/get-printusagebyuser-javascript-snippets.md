---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f86394e1dfd3f6044ac8a17b91256941d8040501d268494110d3d582026b7e7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104942"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printUsageByUser = await client.api('/reports/dailyPrintUsageByUser/{id}')
    .get();

```