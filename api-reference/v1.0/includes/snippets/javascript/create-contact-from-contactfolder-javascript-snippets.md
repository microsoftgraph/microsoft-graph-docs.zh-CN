---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15f04866857b24dbd5de5d2757459e700fe68680ee2aa7e4784d9c2a0ec0333e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219666"
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