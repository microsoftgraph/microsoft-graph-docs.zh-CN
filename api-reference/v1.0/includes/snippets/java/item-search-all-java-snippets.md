---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20bb5dd0e8a6a51352a22e978c27137162e6814f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983073"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveSearchCollectionPage search = graphClient.me().drive()
    .search("Contoso Project")
    .buildRequest()
    .get();

```