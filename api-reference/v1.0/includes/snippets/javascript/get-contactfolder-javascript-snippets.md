---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2692d65dd0e97fd6f636d678543ac50157bf7b6668e40ebe1b6a023a4409b37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contactFolder = await client.api('/me/contactFolders/{id}')
    .get();

```