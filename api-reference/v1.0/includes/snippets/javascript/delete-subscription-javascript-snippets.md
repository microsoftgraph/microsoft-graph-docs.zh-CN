---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebb6f5580da255855ef039c74395f28db935d387129ed850d2251c986573fca7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07')
    .delete();

```