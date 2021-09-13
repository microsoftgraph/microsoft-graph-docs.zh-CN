---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07b548c73359b64c222339840b13df17af09bdc32966ad6ff828c370a7b94376
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106473"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let featureRolloutPolicies = await client.api('/policies/featureRolloutPolicies')
    .get();

```