---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ee541c92e4538c156b0c6ab517520773d119132
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962456"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAgreementCollectionPage agreements = graphClient.agreements()
    .buildRequest()
    .get();

```