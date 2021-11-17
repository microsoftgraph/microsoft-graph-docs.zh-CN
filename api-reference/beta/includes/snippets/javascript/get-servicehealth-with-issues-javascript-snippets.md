---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b814ff8251a400e82055b0f2268f2936c1d043ca47c48ebf7d62fdd11c40337
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332371"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let serviceHealth = await client.api('/admin/serviceAnnouncement/healthOverviews/Microsoft 365 suite')
    .version('beta')
    .expand('issues')
    .get();

```