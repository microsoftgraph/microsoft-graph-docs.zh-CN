---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e920d176d34d3a2afda1eb279a8a1831bc03b69
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982216"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IContactFolderCollectionPage contactFolders = graphClient.me().contactFolders()
    .buildRequest()
    .get();

```