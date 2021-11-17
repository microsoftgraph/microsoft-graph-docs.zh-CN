---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 241e9fe47e001cf9e83279b7ac961ff6234c5f74d15ba69cc9e5f07534f3ba02
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106611"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let healthOverviews = await client.api('/admin/serviceAnnouncement/healthOverviews')
    .version('beta')
    .expand('issues')
    .get();

```