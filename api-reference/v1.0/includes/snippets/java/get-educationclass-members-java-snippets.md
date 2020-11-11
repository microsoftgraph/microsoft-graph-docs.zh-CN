---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1413a803dfbe0fabf731a590fd05025d1d636ad
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48984125"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationUserCollectionWithReferencesPage members = graphClient.education().classes("{class-id}").members()
    .buildRequest()
    .get();

```