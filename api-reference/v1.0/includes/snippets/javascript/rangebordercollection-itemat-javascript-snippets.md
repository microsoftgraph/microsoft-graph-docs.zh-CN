---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef558e1db23345a0f1515291b36de500415178fd102919f6ac2b079e7da65d71
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378415"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeBorder = {
  index: 1
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders/itemAt')
    .post(workbookRangeBorder);

```