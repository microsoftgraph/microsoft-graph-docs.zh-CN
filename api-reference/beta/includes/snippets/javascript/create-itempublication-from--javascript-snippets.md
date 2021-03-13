---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9fe7561e69db48a09654d4237e4c337839dcefc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802124"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemPublication = {
  description: 'One persons journey to the top of the branding management field.',
  displayName: 'Got Brands? The story of Innocenty Popov and his journey to the top.',
  publishedDate: 'Date',
  publisher: 'International Association of Branding Management Publishing',
  thumbnailUrl: 'https://iabm.io/sdhdfhsdhshsd.jpg',
  webUrl: 'https://www.iabm.io'
};

await client.api('/me/profile/publications')
    .version('beta')
    .post(itemPublication);

```