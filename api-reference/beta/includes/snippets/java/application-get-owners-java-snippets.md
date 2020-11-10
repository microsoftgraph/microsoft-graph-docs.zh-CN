---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5cfc27af5eca53a98ec403d6a825869915a25e9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962114"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage owners = graphClient.applications("{id}").owners()
    .buildRequest()
    .get();

```