---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4941b151f7e2b8404ae1a1acd39a813df1847b65
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965194"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage acceptedSenders = graphClient.groups("{id}").acceptedSenders()
    .buildRequest()
    .get();

```