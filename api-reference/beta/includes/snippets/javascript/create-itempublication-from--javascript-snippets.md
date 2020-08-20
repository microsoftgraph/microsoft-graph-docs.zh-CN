---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2e9ab21654790d0ea16bebe940606daba1dd46f
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819731"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemPublication = {
  description: "One persons journey to the top of the branding management field.",
  displayName: "Got Brands? The story of Innocenty Popov and his journey to the top.",
  publishedDate: "Date",
  publisher: "International Association of Branding Management Publishing",
  thumbnailUrl: "https://iabm.io/sdhdfhsdhshsd.jpg",
  webUrl: "https://www.iabm.io"
};

let res = await client.api('/me/profile/publications')
    .version('beta')
    .post(itemPublication);

```