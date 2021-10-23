---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2deb462a3a4696325bd47a5693ccd3472b544e6
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561659"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SubjectRightsRequestCollectionPage subjectRightsRequests = graphClient.privacy().subjectRightsRequests()
    .buildRequest()
    .get();

```