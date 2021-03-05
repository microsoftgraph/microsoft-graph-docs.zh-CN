---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f42f5f09b316b2777d224e04d487c12845b12d6
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470386"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSynchronizationProfile educationSynchronizationProfile = graphClient.education().synchronizationProfiles("{id}")
    .buildRequest()
    .get();

```