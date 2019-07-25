---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2e1c45775861e01cd5f9f1b29cfe05a73da69da7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861542"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveCollectionPage drives = graphClient.groups("{groupId}").drives()
    .buildRequest()
    .get();

```