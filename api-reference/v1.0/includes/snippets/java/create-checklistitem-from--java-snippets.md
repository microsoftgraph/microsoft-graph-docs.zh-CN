---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95b83188d40f151a371a3f4ec91cced2c01e6da6
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66041020"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChecklistItem checklistItem = new ChecklistItem();
checklistItem.displayName = "Final sign-off from the team";

graphClient.me().todo().lists("AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=").tasks("AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA").checklistItems()
    .buildRequest()
    .post(checklistItem);

```