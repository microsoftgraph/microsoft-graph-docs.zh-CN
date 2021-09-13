---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3df89be73702a1286683341c82a9b4b5c46939713d6c62a6d5a8f8dd13ab111
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219933"
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