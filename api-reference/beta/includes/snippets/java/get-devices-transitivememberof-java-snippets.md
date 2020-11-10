---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89bbeb7a1196c07b8bd6bfbc1640b84d9f69c4b0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963493"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage transitiveMemberOf = graphClient.devices("{id}").transitiveMemberOf()
    .buildRequest()
    .get();

```