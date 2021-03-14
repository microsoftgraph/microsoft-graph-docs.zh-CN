---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bed19a6d9ba51ee2d65b30b6cadf43f7b445265
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787748"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directoryRoles/roleTemplateId={role-templateId}/members/{user-id}/$ref')
    .delete();

```