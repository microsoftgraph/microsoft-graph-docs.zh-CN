---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 493dd3a304b11cc0e43355722db99e739a636767
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894080"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveCollectionPage drives = graphClient.users("{userId}").drives()
    .buildRequest()
    .get();

```