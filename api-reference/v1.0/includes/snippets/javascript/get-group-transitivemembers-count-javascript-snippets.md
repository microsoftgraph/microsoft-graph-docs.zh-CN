---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bff0adea879d10a28f83364453f10ec8d4640f64
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209405"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let int32 = await client.api('/groups/{id}/transitiveMembers/$count')
    .header('ConsistencyLevel','eventual')
    .get();

```