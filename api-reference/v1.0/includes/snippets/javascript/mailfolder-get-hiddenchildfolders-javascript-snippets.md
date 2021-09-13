---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d71c890f3f759463cc6f77659289e37edfd9bfb584457576818791a593fc0a4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332337"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let childFolders = await client.api('/me/mailFolders/{id}/childFolders?includeHiddenFolders=true')
    .get();

```