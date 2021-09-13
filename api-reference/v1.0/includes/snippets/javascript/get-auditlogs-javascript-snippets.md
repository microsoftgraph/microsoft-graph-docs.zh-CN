---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6263ea6472de03b17c1380b573946cfd4e7f2c29e753c706a2c26cf8ec10f13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334035"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let auditLogRoot = await client.api('/auditLogs')
    .get();

```