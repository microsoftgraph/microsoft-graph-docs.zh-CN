---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bffb17f8fa71d8d8059c02d6778cb3c5b7117282f9b0765699ccf99fc6a16f93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220623"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/contacts/delta')
    .version('beta')
    .header('Prefer','return=minimal')
    .select('displayName,jobTitle,mail')
    .get();

```