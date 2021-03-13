---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4524b47cf003699f32d52dceb916cdf1d5df0c2f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50769614"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDataSourceCollectionWithReferencesPage custodianSources = graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("{sourceCollectionId}").custodianSources()
    .buildRequest()
    .get();

```