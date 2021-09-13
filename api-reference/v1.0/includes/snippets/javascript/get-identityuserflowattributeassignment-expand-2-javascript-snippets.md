---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0bf8770a3a1c4e7419b651d3f17dd4a319b6f54c71615104418c5dce4859fab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903559"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userAttributeAssignments = await client.api('/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments')
    .expand('userAttribute')
    .get();

```