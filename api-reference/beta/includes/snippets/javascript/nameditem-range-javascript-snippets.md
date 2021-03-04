---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e014952a8d7e5ed754d79b9139ee269a4765b3ca
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442441"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/Range')
    .version('beta')
    .get();

```