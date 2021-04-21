---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8dd60616eab67291034ce6238463cd8c40c04879
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921766"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsAppIcon = await client.api('/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon')
    .version('beta')
    .get();

```