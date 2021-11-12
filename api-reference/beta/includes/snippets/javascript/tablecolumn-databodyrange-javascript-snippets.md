---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aad703428aaebe92c9b79f0b6aaa3059c8122dc7fe830614d708b8085b8cc62b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163350"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/DataBodyRange')
    .version('beta')
    .get();

```