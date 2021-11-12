---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7555dd0145417edcf4b407018f7e4bb14d2aa31b510802afd8f982278ea2d68
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221164"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/contacts/{id}/manager')
    .get();

```