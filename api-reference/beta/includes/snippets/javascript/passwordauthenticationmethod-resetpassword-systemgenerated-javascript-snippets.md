---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4e968c8b89eea1ef99ccfe4407de6f807503e8a
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806008"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/authentication/passwordMethods/{id}/resetPassword')
    .version('beta')
    .post();

```