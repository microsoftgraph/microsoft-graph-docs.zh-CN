---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2bbd229b8df41e87d056fe2952f55ecdef673b9b9def46ece25661c6c8c12ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164184"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let post = await client.api('/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts/AQMkADgAAAIJbQAAAA==')
    .version('beta')
    .get();

```