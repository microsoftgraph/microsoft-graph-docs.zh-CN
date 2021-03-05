---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e156fa9e97a5be50b7def975045e67c5b1bda04
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470463"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationAssignmentResourceCollectionPage resources = graphClient.education().classes("11012").assignments("19002").resources()
    .buildRequest()
    .get();

```