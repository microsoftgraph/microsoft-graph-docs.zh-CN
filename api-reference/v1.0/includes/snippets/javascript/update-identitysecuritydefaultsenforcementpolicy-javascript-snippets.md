---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 172ae19c6772a76114edd80949b9ab46b289c3a54cfb356d6d717cd7c05ea8de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332579"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identitySecurityDefaultsEnforcementPolicy = {
  isEnabled: false
};

await client.api('/policies/identitySecurityDefaultsEnforcementPolicy')
    .update(identitySecurityDefaultsEnforcementPolicy);

```