---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a4cccdd463d03498cb53d9fea838cc22b88783d66c89a44e6831f43e8200cc1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279684"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/directoryObjects/{id}')
    .get();

```