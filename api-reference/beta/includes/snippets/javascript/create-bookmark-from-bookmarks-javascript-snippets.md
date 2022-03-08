---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c4a39505750ad36f3a02c8fb578cca7f676d06e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338243"
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
      languageTag: 'es-ES',
      displayName: 'Sitio de instalación Contoso',
      description: 'Pruebe o compre Contoso hogar o negocios y vea la información del producto'
    }
  ],
  groupIds: ['groupId'],
  powerAppIds: ['powerAppId'],
  state: 'published'
};

await client.api('/search/bookmarks')
    .version('beta')
    .post(bookmark);

```