---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 977c9ddc9855e9048813bc7a8ce36cf713d61eddd58fef3f35e4ac1db6a27417
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333189"
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