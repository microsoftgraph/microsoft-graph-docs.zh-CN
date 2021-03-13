---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4749444d1fc17aec8217c5aeb99e7fe0f683e0c5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772546"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITagAsHierarchyCollectionPage asHierarchy = graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").tags()
    .asHierarchy()
    .buildRequest()
    .get();

```