---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 256a9c19bd0bd7330d7313e4e58baf4a69dad220
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookmark = {
  displayName: 'Contoso Install Site',
  webUrl: 'http://www.contoso.com/',
  description: 'Try or buy Contoso for Home or Business and view product information',
  keywords: {
    keywords: ['Contoso', 'install'],
    reservedKeywords: ['Contoso'],
    matchSimilarKeywords: true
  },
  availabilityStartDateTime: null,
  availabilityEndDateTime: null,
  platforms: ['windows'],
  targetedVariations: [
    {
      languageTag: 'es-es',
      displayName: 'Sitio de instalación Contoso',
      description: 'Pruebe o compre Contoso hogar o negocios y vea la información del producto'
    }
  ],
  state: 'published'
};

await client.api('/search/bookmarks')
    .version('beta')
    .post(bookmark);

```