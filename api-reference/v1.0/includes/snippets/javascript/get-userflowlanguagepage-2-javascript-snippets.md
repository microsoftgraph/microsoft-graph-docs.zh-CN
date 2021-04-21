---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c3482b24ea56bece772de33b5bd83f1fd7fe31a
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920536"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let overridesPages = await client.api('/identity/b2xUserFlows/B2X_1_Partner/languages/en/overridesPages')
    .get();

```