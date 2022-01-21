---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f4ff118789e7b5cf4152146acbca46819a18c57
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111077"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignments = await client.api('/education/users/f3a5344e-dbde-48b0-be24-b5b62a243836/assignments')
    .get();

```