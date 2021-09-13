---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c3da4c175ac2689cd9cc41692a31fab9c6b44a9889dc277a8a7a2831ff84b51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106783"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: 'displayName-value',
};

await client.api('/me/mailFolders/{id}')
    .update(mailFolder);

```