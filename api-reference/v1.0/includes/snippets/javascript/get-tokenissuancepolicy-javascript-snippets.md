---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d84569155dbfee66e64907cb3a1da4f326fa9e06
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779293"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenIssuancePolicy = await client.api('/policies/tokenIssuancepolicies/{id}')
    .get();

```