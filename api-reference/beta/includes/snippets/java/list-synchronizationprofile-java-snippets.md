---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 810c3175755a5b07da543f9af344bb4b2a21e51a6fbd50fb6e732f0bb0abd540
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277460"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSynchronizationProfileCollectionPage synchronizationProfiles = graphClient.education().synchronizationProfiles()
    .buildRequest()
    .get();

```