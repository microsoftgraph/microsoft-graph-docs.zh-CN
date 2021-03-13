---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4bca05c4b8ae1cc602cdaeb227a1b3de00acd4a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tag = {
  description: 'This is an updated description.'
};

await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504')
    .version('beta')
    .update(tag);

```