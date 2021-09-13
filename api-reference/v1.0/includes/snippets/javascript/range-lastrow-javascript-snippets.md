---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9ddcd1a96dcc337fdac239f5bdf6dc5a768d33d0bab7d4d2510f4ae74953dac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221150"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/lastRow')
    .get();

```