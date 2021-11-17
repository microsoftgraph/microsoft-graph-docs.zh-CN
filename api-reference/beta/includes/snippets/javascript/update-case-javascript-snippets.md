---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 767b683a23d667e5c5b52d37e1aa3a7f6f00230ffee9ee6c1b211316dd67a3de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104004"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _case = {
  displayName: 'My Case 1 - Renamed',
  description: 'Updated description',
  externalId: 'Updated externalId'
};

await client.api('/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583')
    .version('beta')
    .update(_case);

```