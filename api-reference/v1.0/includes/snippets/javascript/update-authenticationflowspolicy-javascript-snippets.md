---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9450b68c40ede67a19cf13abc517e2b10ded8b9086bcb569a919943792238689
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationFlowsPolicy = {
  selfServiceSignUp: {
    isEnabled: true
  }
};

await client.api('/policies/authenticationFlowsPolicy')
    .update(authenticationFlowsPolicy);

```