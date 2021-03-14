---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8a3ad8b588e32fa8634085f78ad29dfa2f8d9f4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781970"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members')
    .get();

```