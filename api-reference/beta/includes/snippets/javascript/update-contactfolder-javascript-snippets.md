---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c73d429d74bf2a627338d8ae614c14b4c29691121862b42450f22db1ee990cf1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332741"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contactFolder = {
  parentFolderId: 'parentFolderId-value',
  displayName: 'displayName-value'
};

await client.api('/me/contactFolders/{id}')
    .version('beta')
    .update(contactFolder);

```