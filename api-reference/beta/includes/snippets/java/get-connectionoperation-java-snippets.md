---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1104c3fd4f432c900b5d9ddb6159f151f5dea8dd
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694936"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectionOperation connectionOperation = graphClient.external().connections("contosohr").operations("3ed1595a-4bae-43c2-acda-ef973e581323")
    .buildRequest()
    .get();

```