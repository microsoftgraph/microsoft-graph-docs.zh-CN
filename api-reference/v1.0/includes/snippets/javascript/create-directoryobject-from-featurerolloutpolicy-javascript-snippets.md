---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6632418e6072a7db747345643e2e815e7fc09dc723bcebaabf4763ff9fbb5d59
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221177"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da'
};

await client.api('/policies/featureRolloutPolicies/{id}/appliesTo/$ref')
    .post(directoryObject);

```