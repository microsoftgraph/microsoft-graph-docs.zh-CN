---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5e75a9447a1cd19efdb04f95adaceb507960b43
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225830"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RichLongRunningOperation richLongRunningOperation = graphClient.sites("{siteId}").operations("{richLongRunningOperation-ID}")
    .buildRequest()
    .get();

```