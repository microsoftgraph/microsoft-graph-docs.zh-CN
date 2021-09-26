---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e36c60ee9fcebeead3304c5622cbd06f12e61699
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59765923"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignment educationAssignment = graphClient.education().classes("f4a941ff-9da6-4707-ba5b-0eae93cad0b4").assignments("3c77de7f-539b-49e1-9c96-1274f2f0ee3b")
    .buildRequest()
    .get();

```