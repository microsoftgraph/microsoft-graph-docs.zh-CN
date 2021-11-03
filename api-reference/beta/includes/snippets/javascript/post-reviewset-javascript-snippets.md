---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42e508e004a4143d473d82b5123e2d35dca845058e214cea68a3d81b182f35fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162407"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reviewSet = {
  displayName: 'My Reviewset 3',
};

await client.api('/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets')
    .version('beta')
    .post(reviewSet);

```