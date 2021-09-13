---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e78d178825592b626017532aa0da0a0b14398eb4866f4b378d7039839ee14b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332655"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let claimsMappingPolicies = await client.api('/policies/claimsMappingPolicies')
    .get();

```