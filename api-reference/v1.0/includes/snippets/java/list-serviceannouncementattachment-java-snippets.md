---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 833dbd6b921328cbe718a87f712f318ad46f985a
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225308"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/admin/serviceAnnouncement/messages/MC54091/attachmentsArchive", InputStream.class)
    .buildRequest()
    .get();

```