---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6146105a83ba0edcc5948b3207bb7a5ded9f3316
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981159"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage owners = graphClient.servicePrincipals("{id}").owners()
    .buildRequest()
    .get();

```