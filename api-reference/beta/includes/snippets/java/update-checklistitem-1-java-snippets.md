---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98775aea6199c6f0f0884c58c0890373727a8a08
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66436246"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChecklistItem checklistItem = new ChecklistItem();
checklistItem.displayName = "buy cake";

graphClient.me().todo().lists("AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=").tasks("AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA").checklistItems("e3a26c2e-7c6f-4317-9d71-c27267008202")
    .buildRequest()
    .patch(checklistItem);

```