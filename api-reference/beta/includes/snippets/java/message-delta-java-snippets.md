---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ab8d9824727661245dd7935591a49d98c71d8ae
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981551"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMessageDeltaCollectionPage delta = graphClient.me().mailFolders("{id}").messages()
    .delta()
    .buildRequest()
    .get();

```