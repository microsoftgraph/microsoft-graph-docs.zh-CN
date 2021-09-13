---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ce656ce1fc09a679d69d41fd5012a4f072f5430aa3636773d481a970615906e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let borders = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders')
    .get();

```