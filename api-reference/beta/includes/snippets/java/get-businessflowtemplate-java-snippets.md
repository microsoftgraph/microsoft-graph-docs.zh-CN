---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b0990cace1600669d087620785014c247222126
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960136"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IBusinessFlowTemplateCollectionPage businessFlowTemplates = graphClient.businessFlowTemplates()
    .buildRequest()
    .get();

```