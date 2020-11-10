---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d1599d8ff023c870f771f927a43e4069b7412aa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975510"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOrganizationCollectionPage organization = graphClient.organization()
    .buildRequest()
    .get();

```