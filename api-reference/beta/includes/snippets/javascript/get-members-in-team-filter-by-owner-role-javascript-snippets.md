---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc6f86d14df353e4e5701a6560db6c6c3ae5af9fe02dd750eb774e63e8370656
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members')
    .version('beta')
    .filter('roles/any(r:r eq \'owner\')')
    .get();

```