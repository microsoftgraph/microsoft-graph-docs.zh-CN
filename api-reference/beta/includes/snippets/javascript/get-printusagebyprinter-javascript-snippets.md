---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f75dc91de69f41a7defa0c7247c98fca8e79c09
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869882"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printUsageByPrinter = await client.api('/print/reports/dailyPrintUsageByPrinter/016b5565-3bbf-4067-b9ff-4d68167eb1a6')
    .version('beta')
    .get();

```