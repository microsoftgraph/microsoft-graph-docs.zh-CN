---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b61e2166ace5237bf1cfb38afb3f1e4b79dd8a4f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785162"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRole = await client.api('/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf')
    .get();

```