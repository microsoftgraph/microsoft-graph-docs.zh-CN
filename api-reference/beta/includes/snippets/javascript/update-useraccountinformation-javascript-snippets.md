---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85a7be30fdbd8884b9253e66b05f338f552625ba
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996238"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userAccountInformation = {
  ageGroup: "ageGroup-value",
  countryCode: "countryCode-value",
  preferredLanguageTag: {
    locale: "locale-value",
    displayName: "displayName-value"
  },
  userPrincipalName: "userPrincipalName-value"
};

let res = await client.api('/me/profile/account/{id}')
    .version('beta')
    .update(userAccountInformation);

```