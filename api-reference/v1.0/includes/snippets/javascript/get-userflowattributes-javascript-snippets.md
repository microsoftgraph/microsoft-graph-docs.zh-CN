---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adb748f1bcf3c6b979f30c570d245a57d9b1ef9703259d0d74f5440bdf6308d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378755"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityUserFlowAttribute = await client.api('/identity/userFlowAttributes/{id}')
    .get();

```