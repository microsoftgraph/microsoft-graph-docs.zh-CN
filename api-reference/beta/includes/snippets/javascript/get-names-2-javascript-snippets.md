---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0ecc149d8b7d1b4ee81b926418058b336897b61a78fe9ec44ace11aca8aaf35
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164051"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let names = await client.api('/me/drive/items/{id}/workbook/names')
    .version('beta')
    .get();

```