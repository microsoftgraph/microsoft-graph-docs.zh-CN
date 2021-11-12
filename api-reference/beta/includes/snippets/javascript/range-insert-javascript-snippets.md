---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59ce982587fa5b0797b2a0ed681edc7a9200bff87a29011adb70fa4c030e03c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107138"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRange = {
  shift: 'shift-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/insert')
    .version('beta')
    .post(workbookRange);

```