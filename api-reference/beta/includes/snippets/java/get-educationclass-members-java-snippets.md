---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de0ec9659891d95f9e1e41edef7c5fd9cbd61182
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966270"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationUserCollectionWithReferencesPage members = graphClient.education().classes("11016").members()
    .buildRequest()
    .get();

```