---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f4bcf3282db9db17853bed713d4148c2e43b852b59b6e6f74c79c45b45ee07b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104892"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartAxisTitle = {
  text: 'text-value',
  visible: true
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title')
    .version('beta')
    .update(workbookChartAxisTitle);

```