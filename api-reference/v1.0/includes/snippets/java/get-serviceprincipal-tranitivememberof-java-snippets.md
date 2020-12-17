---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3875a8e502e43618cf15402807c55c5502ab5376
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983269"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage transitiveMemberOf = graphClient.servicePrincipals("{id}").transitiveMemberOf()
    .buildRequest()
    .get();

```