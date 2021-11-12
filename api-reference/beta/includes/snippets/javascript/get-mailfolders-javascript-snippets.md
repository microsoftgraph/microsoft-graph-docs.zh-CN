---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44d01e8c9ae73c88a80bb07122dc28f8266de82cc5c3b46bb4d72c569cdb6404
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162692"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mailFolders = await client.api('/me/mailFolders')
    .version('beta')
    .get();

```