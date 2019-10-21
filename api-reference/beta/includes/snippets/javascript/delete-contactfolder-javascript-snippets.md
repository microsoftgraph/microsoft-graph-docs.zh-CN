---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbc07441eb6d9c75cae0124713be26fa029f85d7
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "35707487"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/{id}')
    .version('beta')
    .delete();

```