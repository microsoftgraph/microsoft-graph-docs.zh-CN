---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03877751d797b5800568b0319368792bd40027ee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977519"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = graphClient.education().classes("{class-id}")
    .buildRequest()
    .get();

```