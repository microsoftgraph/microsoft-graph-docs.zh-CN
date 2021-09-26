---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 691f07bbfd51b280ef32d533fd194a0340b9066cf10c22ec14f8ec67d5dac79f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278397"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _case = {
    displayName: 'My Case 1',
};

await client.api('/compliance/ediscovery/cases')
    .version('beta')
    .post(_case);

```