---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c6d2dac379c7c21a410eb9c4ab5f1a7b8747ee8a62057dc8907084597c3531f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279366"
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
    .update(contactFolder);

```