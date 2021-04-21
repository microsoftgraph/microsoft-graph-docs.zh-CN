---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a68fe1277cd30d9f42cdd7524f2a5edfddf2c5d3
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921763"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsAppIcon = await client.api('/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon')
    .version('beta')
    .get();

```