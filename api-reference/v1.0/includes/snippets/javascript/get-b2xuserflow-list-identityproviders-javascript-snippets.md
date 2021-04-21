---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4e680cd26dafc23c1d632170b801bedcc04b321
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919931"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviders = await client.api('/identity/b2xUserFlows/B2X_1_Partner/identityProviders')
    .get();

```