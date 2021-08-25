---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37f1a3944b292e44647683f0a0ba2362558b469bf61bddb6c620eafc8731bf22
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215639"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let posts = await client.api('/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts')
    .version('beta')
    .get();

```