---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54db040ebc5d425aeab43abd983945290db06cae
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440957"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  description: "Member of the Microsoft API Council",
  displayName: "API Council",
  collaborationTags: [
    "askMeAbout"
  ]
};

let res = await client.api('/me/responsibilities')
    .version('beta')
    .post(string);

```