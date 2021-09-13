---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29921bdf2dc4636797c6d21acfa3660fcbe82bae677d6fbc79263f9c8757b164
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221390"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/lastColumn')
    .get();

```