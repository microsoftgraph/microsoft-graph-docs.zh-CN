---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06a536bc0aa27246e4b300b6ae49b6e7c2c10b8c9356eb6109427af7b1b5dbe2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162359"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appRoleAssignment = {
  principalId: '9028d19c-26a9-4809-8e3f-20ff73e2d75e',
  resourceId: '8fce32da-1246-437b-99cd-76d1d4677bd5',
  appRoleId: '498476ce-e0fe-48b0-b801-37ba7e2685c6'
};

await client.api('/servicePrincipals/9028d19c-26a9-4809-8e3f-20ff73e2d75e/appRoleAssignments')
    .post(appRoleAssignment);

```