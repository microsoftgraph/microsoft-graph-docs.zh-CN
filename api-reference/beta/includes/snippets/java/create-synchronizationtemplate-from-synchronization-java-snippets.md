---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 665e81c8a36afc0e01cb064e9b6c6bf37f5dfd69
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978422"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationTemplate synchronizationTemplate = new SynchronizationTemplate();
synchronizationTemplate.id = "SCIM-Test1";
synchronizationTemplate.applicationId = UUID.fromString("{id}");
synchronizationTemplate.factoryTag = "CustomSCIM";

graphClient.applications("{id}").synchronization().templates()
    .buildRequest()
    .post(synchronizationTemplate);

```