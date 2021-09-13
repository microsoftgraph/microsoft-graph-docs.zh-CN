---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f3635171b4a475f1cab24b05d6f040f0bd0fafead33d6a6e02872ff43c7d4ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162994"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookFormatProtection = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/protection')
    .get();

```