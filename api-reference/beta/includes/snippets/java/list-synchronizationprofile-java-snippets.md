---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65218db8ed637f1b51035b499cfed317feb98e8a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470500"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationSynchronizationProfileCollectionPage synchronizationProfiles = graphClient.education().synchronizationProfiles()
    .buildRequest()
    .get();

```