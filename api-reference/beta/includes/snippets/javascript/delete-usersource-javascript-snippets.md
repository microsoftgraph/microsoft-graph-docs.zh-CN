---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d67454e7af34066bfb4973ec064d6e39f67ca28
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657214"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735')
    .version('beta')
    .delete();

```