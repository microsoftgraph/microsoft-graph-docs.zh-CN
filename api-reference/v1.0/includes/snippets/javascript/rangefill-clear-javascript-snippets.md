---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 290e505d7dc600681295aa5d92c7bbeb3ae8218b0b67e49bf687511a69779c0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902953"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill/clear')
    .post();

```