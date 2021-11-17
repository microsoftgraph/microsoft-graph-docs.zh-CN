---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8c4a425f205b7f20350759b6e88847f959b7f6df48ea34efa057991e9bfbbe3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personWebsite = {
  description: 'Lyn Damer play in the Women\'s 1st Division (Toppserien) in Norway'
};

await client.api('/me/profile/websites/{id}')
    .version('beta')
    .update(personWebsite);

```