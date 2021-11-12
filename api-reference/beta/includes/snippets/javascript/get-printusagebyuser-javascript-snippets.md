---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1ec7378af8449cc38c0ca2d8992975362686a5acc145bff5da9e91da866a3d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333448"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printUsageByUser = await client.api('/print/reports/dailyPrintUsageByUser/016b5565-3bbf-4067-b9ff-4d68167eb1a6')
    .version('beta')
    .get();

```