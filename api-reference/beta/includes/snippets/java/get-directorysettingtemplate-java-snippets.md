---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74c761830323b74f7db1339b3aad107b61ff9dff
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514484"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectorySettingTemplate directorySettingTemplate = graphClient.directorySettingTemplates("08d542b9-071f-4e16-94b0-74abb372e3d9")
    .buildRequest()
    .get();

```