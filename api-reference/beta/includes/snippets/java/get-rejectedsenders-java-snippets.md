---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a9c8b2b983d4b1f6795f80991950f182e4d3f26
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093540"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage rejectedSenders = graphClient.groups("{id}").rejectedSenders()
    .buildRequest()
    .get();

```