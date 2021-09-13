---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4edd3233407d8d0560832c4caafae7bdda0f0010b2370412a5a05d921ef10f74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274066"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookFormatProtection = {
  locked: true,
  formulaHidden: true
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/protection')
    .update(workbookFormatProtection);

```