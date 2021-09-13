---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed9b8cef15d5d3bdf7c3f312460bba0a7dbd574e6df51abe0590a7458f46c87c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332103"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/claimsMappingPolicies/{id}/appliesTo')
    .get();

```