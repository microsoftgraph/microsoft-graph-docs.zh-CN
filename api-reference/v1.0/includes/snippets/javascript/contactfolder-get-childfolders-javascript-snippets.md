---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33790078ed54ffac13bec3086767fc669d0b2d0f20115fa9c121b9d8055cce29
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104619"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let childFolders = await client.api('/me/contactFolders/{id}/childFolders')
    .get();

```