---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1aa61b404b095ff3b3da5b6baac4ef17f41f9861ae5918a01d6a0aa33d26ba4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378401"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/EntireColumn')
    .version('beta')
    .get();

```