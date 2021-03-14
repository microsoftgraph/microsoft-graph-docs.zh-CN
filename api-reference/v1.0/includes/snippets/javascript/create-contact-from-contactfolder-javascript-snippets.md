---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14dc6f0f57b043e18bcfd065ee4dbf79241fb6df
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805937"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
  parentFolderId: 'parentFolderId-value',
  birthday: 'datetime-value',
  fileAs: 'fileAs-value',
  displayName: 'displayName-value',
  givenName: 'givenName-value',
  initials: 'initials-value'
};

await client.api('/me/contactFolders/{id}/contacts')
    .post(contact);

```