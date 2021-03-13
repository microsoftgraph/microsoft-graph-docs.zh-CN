---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 988ce634328ea28799cebf7304c213ec13dfaa7a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770361"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemPublication = {
  publisher: 'International Association of Branding Management Publishing',
  thumbnailUrl: 'https://iabm.io/sdhdfhsdhshsd.jpg',
};

await client.api('/users/{userId}/profile/publications/{id}')
    .version('beta')
    .update(itemPublication);

```