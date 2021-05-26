---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 649d9f8631a1c79b3afca81426402eac662de4c8
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52663976"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationContextClassReferenceCollectionPage authenticationContextClassReferences = graphClient.identity().conditionalAccess().authenticationContextClassReferences()
    .buildRequest()
    .get();

```