---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 757f466cfa87aecc6ec54dbdd6e72d8465a66519dc704c6f44ade8b929718aca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328957"
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